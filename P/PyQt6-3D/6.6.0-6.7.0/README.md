# Comparing `tmp/PyQt6_3D-6.6.0.tar.gz` & `tmp/PyQt6_3D-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_3D-6.6.0.tar", last modified: Wed Oct 25 10:21:14 2023, max compression
+gzip compressed data, was "PyQt6_3D-6.7.0.tar", last modified: Sat Apr 20 16:01:00 2024, max compression
```

## Comparing `PyQt6_3D-6.6.0.tar` & `PyQt6_3D-6.7.0.tar`

### file list

```diff
@@ -1,355 +1,355 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.207277 PyQt6_3D-6.6.0/
--rw-r--r--   0 phil       (501) staff       (20)    10232 2023-10-25 10:21:12.634297 PyQt6_3D-6.6.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-10-25 10:21:12.400798 PyQt6_3D-6.6.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      690 2023-10-25 10:16:21.970561 PyQt6_3D-6.6.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1578 2023-10-25 10:21:14.207421 PyQt6_3D-6.6.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1265 2023-10-25 10:21:12.635747 PyQt6_3D-6.6.0/README
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.056567 PyQt6_3D-6.6.0/examples/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.086275 PyQt6_3D-6.6.0/examples/assets/
--rw-r--r--   0 phil       (501) staff       (20)      136 2023-10-25 10:16:21.982623 PyQt6_3D-6.6.0/examples/assets/LICENSE
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.085849 PyQt6_3D-6.6.0/examples/assets/chest/
--rw-r--r--   0 phil       (501) staff       (20)    46344 2023-10-25 10:16:21.984415 PyQt6_3D-6.6.0/examples/assets/chest/Chest.obj
--rw-r--r--   0 phil       (501) staff       (20)    70980 2023-10-25 10:16:21.985995 PyQt6_3D-6.6.0/examples/assets/chest/diffuse.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.067246 PyQt6_3D-6.6.0/examples/assets/cubemaps/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.066831 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/
--rw-r--r--   0 phil       (501) staff       (20)      293 2023-10-25 10:16:21.987090 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/README.TXT
--rw-r--r--   0 phil       (501) staff       (20)   121754 2023-10-25 10:16:21.990328 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_negx.webp
--rw-r--r--   0 phil       (501) staff       (20)     1926 2023-10-25 10:16:21.991675 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_negy.webp
--rw-r--r--   0 phil       (501) staff       (20)   147696 2023-10-25 10:16:21.994729 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_negz.webp
--rw-r--r--   0 phil       (501) staff       (20)   136426 2023-10-25 10:16:21.997603 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_posx.webp
--rw-r--r--   0 phil       (501) staff       (20)    57622 2023-10-25 10:16:21.999101 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_posy.webp
--rw-r--r--   0 phil       (501) staff       (20)   164564 2023-10-25 10:16:22.002031 PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_posz.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.069542 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/
--rw-r--r--   0 phil       (501) staff       (20)    38042 2023-10-25 10:16:22.003711 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_negx.webp
--rw-r--r--   0 phil       (501) staff       (20)    42278 2023-10-25 10:16:22.004854 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_negy.webp
--rw-r--r--   0 phil       (501) staff       (20)    36790 2023-10-25 10:16:22.006343 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_negz.webp
--rw-r--r--   0 phil       (501) staff       (20)    37092 2023-10-25 10:16:22.008028 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_posx.webp
--rw-r--r--   0 phil       (501) staff       (20)    26008 2023-10-25 10:16:22.009119 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_posy.webp
--rw-r--r--   0 phil       (501) staff       (20)    37802 2023-10-25 10:16:22.010171 PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_posz.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.070490 PyQt6_3D-6.6.0/examples/assets/gltf/
--rw-r--r--   0 phil       (501) staff       (20)     1831 2023-10-25 10:16:22.011191 PyQt6_3D-6.6.0/examples/assets/gltf/LICENSE.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.077218 PyQt6_3D-6.6.0/examples/assets/gltf/wine/
--rw-r--r--   0 phil       (501) staff       (20)     8798 2023-10-25 10:16:22.012723 PyQt6_3D-6.6.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg
--rw-r--r--   0 phil       (501) staff       (20)    46051 2023-10-25 10:16:22.014621 PyQt6_3D-6.6.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg
--rw-r--r--   0 phil       (501) staff       (20)    35585 2023-10-25 10:16:22.016449 PyQt6_3D-6.6.0/examples/assets/gltf/wine/artezin_bottle.jpg
--rw-r--r--   0 phil       (501) staff       (20)   329088 2023-10-25 10:16:22.020712 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine.bin
--rw-r--r--   0 phil       (501) staff       (20)   797366 2023-10-25 10:16:22.028574 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine.dae
--rw-r--r--   0 phil       (501) staff       (20)   275432 2023-10-25 10:16:22.031333 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine.gltf
--rw-r--r--   0 phil       (501) staff       (20)      497 2023-10-25 10:16:22.032775 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine0FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      439 2023-10-25 10:16:22.034103 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine0VS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      489 2023-10-25 10:16:22.035156 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine1FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      355 2023-10-25 10:16:22.036196 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine1VS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      219 2023-10-25 10:16:22.037245 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine2FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      236 2023-10-25 10:16:22.038281 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine2VS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      441 2023-10-25 10:16:22.039446 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine3FS.glsl
--rw-r--r--   0 phil       (501) staff       (20)      355 2023-10-25 10:16:22.040462 PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine3VS.glsl
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.120855 PyQt6_3D-6.6.0/examples/assets/houseplants/
--rw-r--r--   0 phil       (501) staff       (20)    13846 2023-10-25 10:16:22.041771 PyQt6_3D-6.6.0/examples/assets/houseplants/bamboo.webp
--rw-r--r--   0 phil       (501) staff       (20)    16614 2023-10-25 10:16:22.042785 PyQt6_3D-6.6.0/examples/assets/houseplants/bamboo_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    89192 2023-10-25 10:16:22.044630 PyQt6_3D-6.6.0/examples/assets/houseplants/cover.webp
--rw-r--r--   0 phil       (501) staff       (20)    21098 2023-10-25 10:16:22.045974 PyQt6_3D-6.6.0/examples/assets/houseplants/cover_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    44264 2023-10-25 10:16:22.047695 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36076 2023-10-25 10:16:22.049352 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9324 2023-10-25 10:16:22.050925 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1822 2023-10-25 10:16:22.052271 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     8863 2023-10-25 10:16:22.053332 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15838 2023-10-25 10:16:22.054890 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2216 2023-10-25 10:16:22.055887 PyQt6_3D-6.6.0/examples/assets/houseplants/cross-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    51505 2023-10-25 10:16:22.057171 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36078 2023-10-25 10:16:22.058542 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2023-10-25 10:16:22.059482 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1820 2023-10-25 10:16:22.060709 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     9026 2023-10-25 10:16:22.061985 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2023-10-25 10:16:22.063446 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2216 2023-10-25 10:16:22.064411 PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    33756 2023-10-25 10:16:22.065447 PyQt6_3D-6.6.0/examples/assets/houseplants/palm.webp
--rw-r--r--   0 phil       (501) staff       (20)    36186 2023-10-25 10:16:22.066463 PyQt6_3D-6.6.0/examples/assets/houseplants/palm_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)   120426 2023-10-25 10:16:22.068350 PyQt6_3D-6.6.0/examples/assets/houseplants/pine.webp
--rw-r--r--   0 phil       (501) staff       (20)    47352 2023-10-25 10:16:22.070023 PyQt6_3D-6.6.0/examples/assets/houseplants/pine_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)   366144 2023-10-25 10:16:22.073775 PyQt6_3D-6.6.0/examples/assets/houseplants/pot.webp
--rw-r--r--   0 phil       (501) staff       (20)    50950 2023-10-25 10:16:22.076639 PyQt6_3D-6.6.0/examples/assets/houseplants/pot_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    33100 2023-10-25 10:16:22.078193 PyQt6_3D-6.6.0/examples/assets/houseplants/shrub.webp
--rw-r--r--   0 phil       (501) staff       (20)    10180 2023-10-25 10:16:22.079612 PyQt6_3D-6.6.0/examples/assets/houseplants/shrub_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    51509 2023-10-25 10:16:22.081467 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36082 2023-10-25 10:16:22.083104 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2023-10-25 10:16:22.084603 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1820 2023-10-25 10:16:22.086011 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)    46455 2023-10-25 10:16:22.087837 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2023-10-25 10:16:22.089354 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2220 2023-10-25 10:16:22.090303 PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    30338 2023-10-25 10:16:22.091248 PyQt6_3D-6.6.0/examples/assets/houseplants/spikes.webp
--rw-r--r--   0 phil       (501) staff       (20)    12028 2023-10-25 10:16:22.092620 PyQt6_3D-6.6.0/examples/assets/houseplants/spikes_normal.webp
--rw-r--r--   0 phil       (501) staff       (20)    51509 2023-10-25 10:16:22.094098 PyQt6_3D-6.6.0/examples/assets/houseplants/square-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36082 2023-10-25 10:16:22.095803 PyQt6_3D-6.6.0/examples/assets/houseplants/square-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2023-10-25 10:16:22.096837 PyQt6_3D-6.6.0/examples/assets/houseplants/square-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1824 2023-10-25 10:16:22.098172 PyQt6_3D-6.6.0/examples/assets/houseplants/square-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     3725 2023-10-25 10:16:22.099694 PyQt6_3D-6.6.0/examples/assets/houseplants/square-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2023-10-25 10:16:22.101262 PyQt6_3D-6.6.0/examples/assets/houseplants/square-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2220 2023-10-25 10:16:22.102265 PyQt6_3D-6.6.0/examples/assets/houseplants/square-spikes.obj
--rw-r--r--   0 phil       (501) staff       (20)    28687 2023-10-25 10:16:22.103861 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-bamboo.obj
--rw-r--r--   0 phil       (501) staff       (20)    36082 2023-10-25 10:16:22.105558 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-palm.obj
--rw-r--r--   0 phil       (501) staff       (20)     9328 2023-10-25 10:16:22.106543 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-pine.obj
--rw-r--r--   0 phil       (501) staff       (20)     1808 2023-10-25 10:16:22.107415 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-pot-cover.obj
--rw-r--r--   0 phil       (501) staff       (20)     2469 2023-10-25 10:16:22.108296 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-pot.obj
--rw-r--r--   0 phil       (501) staff       (20)    15842 2023-10-25 10:16:22.109722 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-shrub.obj
--rw-r--r--   0 phil       (501) staff       (20)     2220 2023-10-25 10:16:22.110696 PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-spikes.obj
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.084885 PyQt6_3D-6.6.0/examples/assets/metalbarrel/
--rw-r--r--   0 phil       (501) staff       (20)   162040 2023-10-25 10:16:22.113496 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_black.webp
--rw-r--r--   0 phil       (501) staff       (20)   101158 2023-10-25 10:16:22.115261 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_blue.webp
--rw-r--r--   0 phil       (501) staff       (20)    74498 2023-10-25 10:16:22.117043 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_green.webp
--rw-r--r--   0 phil       (501) staff       (20)    86874 2023-10-25 10:16:22.118838 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_red.webp
--rw-r--r--   0 phil       (501) staff       (20)   254934 2023-10-25 10:16:22.122180 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_rust.webp
--rw-r--r--   0 phil       (501) staff       (20)     6042 2023-10-25 10:16:22.123629 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_stainless_steel.webp
--rw-r--r--   0 phil       (501) staff       (20)   101134 2023-10-25 10:16:22.125569 PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_yellow.webp
--rw-r--r--   0 phil       (501) staff       (20)    27126 2023-10-25 10:16:22.126877 PyQt6_3D-6.6.0/examples/assets/metalbarrel/metal_barrel.obj
--rw-r--r--   0 phil       (501) staff       (20)    29446 2023-10-25 10:16:22.128321 PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_hard_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)    25560 2023-10-25 10:16:22.129869 PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_middle_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)    21544 2023-10-25 10:16:22.131587 PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_no_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)    23620 2023-10-25 10:16:22.133209 PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_soft_bumps.webp
--rw-r--r--   0 phil       (501) staff       (20)   420416 2023-10-25 10:16:22.137370 PyQt6_3D-6.6.0/examples/assets/metalbarrel/specular.webp
--rw-r--r--   0 phil       (501) staff       (20)   330298 2023-10-25 10:16:22.141017 PyQt6_3D-6.6.0/examples/assets/metalbarrel/specular_rust.webp
--rw-r--r--   0 phil       (501) staff       (20)   220224 2023-10-25 10:16:22.144811 PyQt6_3D-6.6.0/examples/assets/metalbarrel/specular_stainless_steel.webp
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.059873 PyQt6_3D-6.6.0/examples/assets/obj/
--rw-r--r--   0 phil       (501) staff       (20)   346814 2023-10-25 10:16:22.149012 PyQt6_3D-6.6.0/examples/assets/obj/ball.obj
--rw-r--r--   0 phil       (501) staff       (20)  1764501 2023-10-25 10:16:22.165632 PyQt6_3D-6.6.0/examples/assets/obj/toyplane.obj
--rw-r--r--   0 phil       (501) staff       (20)   263373 2023-10-25 10:16:22.169054 PyQt6_3D-6.6.0/examples/assets/obj/trefoil.obj
--rw-r--r--   0 phil       (501) staff       (20)   127711 2023-10-25 10:16:22.171163 PyQt6_3D-6.6.0/examples/assets/test_scene.dae
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.060542 PyQt6_3D-6.6.0/examples/assets/textures/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.063023 PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/
--rw-r--r--   0 phil       (501) staff       (20)   677322 2023-10-25 10:16:22.179622 PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/diffuse.webp
--rw-r--r--   0 phil       (501) staff       (20)   822594 2023-10-25 10:16:22.185079 PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/normal.webp
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-10-25 10:16:22.185867 PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/readme.txt
--rw-r--r--   0 phil       (501) staff       (20)  1005334 2023-10-25 10:16:22.194499 PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/specular.webp
--rw-r--r--   0 phil       (501) staff       (20)    10285 2023-10-25 10:16:22.195666 PyQt6_3D-6.6.0/examples/basicshapes-py.py
--rw-r--r--   0 phil       (501) staff       (20)    18568 2023-10-25 10:16:22.196948 PyQt6_3D-6.6.0/examples/materials-py.py
--rw-r--r--   0 phil       (501) staff       (20)     6082 2023-10-25 10:16:22.197888 PyQt6_3D-6.6.0/examples/simple-py.py
--rw-r--r--   0 phil       (501) staff       (20)     1072 2023-10-25 10:21:12.636312 PyQt6_3D-6.6.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.169215 PyQt6_3D-6.6.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.168801 PyQt6_3D-6.6.0/sip/Qt3DAnimation/
--rw-r--r--   0 phil       (501) staff       (20)     2857 2023-10-25 10:21:13.754039 PyQt6_3D-6.6.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     4844 2023-10-25 10:21:13.756413 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1344 2023-10-25 10:21:13.753471 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractanimationclip.sip
--rw-r--r--   0 phil       (501) staff       (20)     1257 2023-10-25 10:21:13.742371 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractchannelmapping.sip
--rw-r--r--   0 phil       (501) staff       (20)     2214 2023-10-25 10:21:13.743546 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractclipanimator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1336 2023-10-25 10:21:13.754521 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractclipblendnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1959 2023-10-25 10:21:13.745765 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qadditiveclipblend.sip
--rw-r--r--   0 phil       (501) staff       (20)     1286 2023-10-25 10:21:13.746903 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1538 2023-10-25 10:21:13.750742 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationclip.sip
--rw-r--r--   0 phil       (501) staff       (20)     1631 2023-10-25 10:21:13.748487 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationclipdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1848 2023-10-25 10:21:13.744143 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationcliploader.sip
--rw-r--r--   0 phil       (501) staff       (20)     2530 2023-10-25 10:21:13.749072 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationcontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1884 2023-10-25 10:21:13.741873 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationgroup.sip
--rw-r--r--   0 phil       (501) staff       (20)     1605 2023-10-25 10:21:13.742918 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qblendedclipanimator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1724 2023-10-25 10:21:13.751825 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannel.sip
--rw-r--r--   0 phil       (501) staff       (20)     1659 2023-10-25 10:21:13.744691 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannelcomponent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1497 2023-10-25 10:21:13.747454 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1758 2023-10-25 10:21:13.746365 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannelmapping.sip
--rw-r--r--   0 phil       (501) staff       (20)     1519 2023-10-25 10:21:13.752978 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qclipanimator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1646 2023-10-25 10:21:13.745217 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qclipblendvalue.sip
--rw-r--r--   0 phil       (501) staff       (20)     1381 2023-10-25 10:21:13.747954 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qclock.sip
--rw-r--r--   0 phil       (501) staff       (20)     2025 2023-10-25 10:21:13.755124 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qkeyframe.sip
--rw-r--r--   0 phil       (501) staff       (20)     2787 2023-10-25 10:21:13.752460 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qkeyframeanimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1900 2023-10-25 10:21:13.741226 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qlerpclipblend.sip
--rw-r--r--   0 phil       (501) staff       (20)     2779 2023-10-25 10:21:13.749688 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qmorphinganimation.sip
--rw-r--r--   0 phil       (501) staff       (20)     1721 2023-10-25 10:21:13.750197 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qmorphtarget.sip
--rw-r--r--   0 phil       (501) staff       (20)     1529 2023-10-25 10:21:13.755608 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qskeletonmapping.sip
--rw-r--r--   0 phil       (501) staff       (20)     2199 2023-10-25 10:21:13.751280 PyQt6_3D-6.6.0/sip/Qt3DAnimation/qvertexblendanimation.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.130719 PyQt6_3D-6.6.0/sip/Qt3DCore/
--rw-r--r--   0 phil       (501) staff       (20)     2751 2023-10-25 10:21:13.690790 PyQt6_3D-6.6.0/sip/Qt3DCore/Qt3DCoremod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1557 2023-10-25 10:21:13.691438 PyQt6_3D-6.6.0/sip/Qt3DCore/qabstractaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1262 2023-10-25 10:21:13.684080 PyQt6_3D-6.6.0/sip/Qt3DCore/qabstractfunctor.sip
--rw-r--r--   0 phil       (501) staff       (20)     1311 2023-10-25 10:21:13.692026 PyQt6_3D-6.6.0/sip/Qt3DCore/qabstractskeleton.sip
--rw-r--r--   0 phil       (501) staff       (20)     1459 2023-10-25 10:21:13.681825 PyQt6_3D-6.6.0/sip/Qt3DCore/qarmature.sip
--rw-r--r--   0 phil       (501) staff       (20)     2108 2023-10-25 10:21:13.684811 PyQt6_3D-6.6.0/sip/Qt3DCore/qaspectengine.sip
--rw-r--r--   0 phil       (501) staff       (20)     4235 2023-10-25 10:21:13.692974 PyQt6_3D-6.6.0/sip/Qt3DCore/qattribute.sip
--rw-r--r--   0 phil       (501) staff       (20)     2024 2023-10-25 10:21:13.695102 PyQt6_3D-6.6.0/sip/Qt3DCore/qbackendnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     2124 2023-10-25 10:21:13.694303 PyQt6_3D-6.6.0/sip/Qt3DCore/qboundingvolume.sip
--rw-r--r--   0 phil       (501) staff       (20)     2252 2023-10-25 10:21:13.680267 PyQt6_3D-6.6.0/sip/Qt3DCore/qbuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1604 2023-10-25 10:21:13.686363 PyQt6_3D-6.6.0/sip/Qt3DCore/qcomponent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1481 2023-10-25 10:21:13.682464 PyQt6_3D-6.6.0/sip/Qt3DCore/qcoresettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1740 2023-10-25 10:21:13.685476 PyQt6_3D-6.6.0/sip/Qt3DCore/qentity.sip
--rw-r--r--   0 phil       (501) staff       (20)     2182 2023-10-25 10:21:13.688273 PyQt6_3D-6.6.0/sip/Qt3DCore/qgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     3346 2023-10-25 10:21:13.681176 PyQt6_3D-6.6.0/sip/Qt3DCore/qgeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     2574 2023-10-25 10:21:13.679454 PyQt6_3D-6.6.0/sip/Qt3DCore/qjoint.sip
--rw-r--r--   0 phil       (501) staff       (20)     4044 2023-10-25 10:21:13.683478 PyQt6_3D-6.6.0/sip/Qt3DCore/qnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1631 2023-10-25 10:21:13.693616 PyQt6_3D-6.6.0/sip/Qt3DCore/qnodeid.sip
--rw-r--r--   0 phil       (501) staff       (20)     3247 2023-10-25 10:21:13.687533 PyQt6_3D-6.6.0/sip/Qt3DCore/qsharedpointer.sip
--rw-r--r--   0 phil       (501) staff       (20)     1429 2023-10-25 10:21:13.688928 PyQt6_3D-6.6.0/sip/Qt3DCore/qskeleton.sip
--rw-r--r--   0 phil       (501) staff       (20)     2040 2023-10-25 10:21:13.695828 PyQt6_3D-6.6.0/sip/Qt3DCore/qskeletonloader.sip
--rw-r--r--   0 phil       (501) staff       (20)     3350 2023-10-25 10:21:13.690004 PyQt6_3D-6.6.0/sip/Qt3DCore/qtransform.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.158174 PyQt6_3D-6.6.0/sip/Qt3DExtras/
--rw-r--r--   0 phil       (501) staff       (20)     3472 2023-10-25 10:21:13.738605 PyQt6_3D-6.6.0/sip/Qt3DExtras/Qt3DExtrasmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2125 2023-10-25 10:21:13.722788 PyQt6_3D-6.6.0/sip/Qt3DExtras/qabstractcameracontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1709 2023-10-25 10:21:13.725750 PyQt6_3D-6.6.0/sip/Qt3DExtras/qabstractspritesheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     2448 2023-10-25 10:21:13.716736 PyQt6_3D-6.6.0/sip/Qt3DExtras/qconegeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2192 2023-10-25 10:21:13.739239 PyQt6_3D-6.6.0/sip/Qt3DExtras/qconegeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     2150 2023-10-25 10:21:13.715299 PyQt6_3D-6.6.0/sip/Qt3DExtras/qconemesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     2498 2023-10-25 10:21:13.720241 PyQt6_3D-6.6.0/sip/Qt3DExtras/qcuboidgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     2186 2023-10-25 10:21:13.724032 PyQt6_3D-6.6.0/sip/Qt3DExtras/qcuboidgeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     2144 2023-10-25 10:21:13.739873 PyQt6_3D-6.6.0/sip/Qt3DExtras/qcuboidmesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     2028 2023-10-25 10:21:13.718467 PyQt6_3D-6.6.0/sip/Qt3DExtras/qcylindergeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1772 2023-10-25 10:21:13.721506 PyQt6_3D-6.6.0/sip/Qt3DExtras/qcylindergeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1730 2023-10-25 10:21:13.740484 PyQt6_3D-6.6.0/sip/Qt3DExtras/qcylindermesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     2070 2023-10-25 10:21:13.713193 PyQt6_3D-6.6.0/sip/Qt3DExtras/qdiffusemapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2191 2023-10-25 10:21:13.734234 PyQt6_3D-6.6.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2329 2023-10-25 10:21:13.713845 PyQt6_3D-6.6.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1880 2023-10-25 10:21:13.737214 PyQt6_3D-6.6.0/sip/Qt3DExtras/qextrudedtextgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1670 2023-10-25 10:21:13.735333 PyQt6_3D-6.6.0/sip/Qt3DExtras/qextrudedtextmesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1372 2023-10-25 10:21:13.733054 PyQt6_3D-6.6.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     2847 2023-10-25 10:21:13.714615 PyQt6_3D-6.6.0/sip/Qt3DExtras/qforwardrenderer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2138 2023-10-25 10:21:13.722153 PyQt6_3D-6.6.0/sip/Qt3DExtras/qgoochmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2235 2023-10-25 10:21:13.730436 PyQt6_3D-6.6.0/sip/Qt3DExtras/qmetalroughmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2001 2023-10-25 10:21:13.728601 PyQt6_3D-6.6.0/sip/Qt3DExtras/qmorphphongmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1384 2023-10-25 10:21:13.717256 PyQt6_3D-6.6.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2306 2023-10-25 10:21:13.717865 PyQt6_3D-6.6.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2425 2023-10-25 10:21:13.729240 PyQt6_3D-6.6.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1468 2023-10-25 10:21:13.734776 PyQt6_3D-6.6.0/sip/Qt3DExtras/qorbitcameracontroller.sip
--rw-r--r--   0 phil       (501) staff       (20)     1326 2023-10-25 10:21:13.719006 PyQt6_3D-6.6.0/sip/Qt3DExtras/qpervertexcolormaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     3390 2023-10-25 10:21:13.716075 PyQt6_3D-6.6.0/sip/Qt3DExtras/qphongalphamaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     1831 2023-10-25 10:21:13.727484 PyQt6_3D-6.6.0/sip/Qt3DExtras/qphongmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2119 2023-10-25 10:21:13.732550 PyQt6_3D-6.6.0/sip/Qt3DExtras/qplanegeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1823 2023-10-25 10:21:13.733632 PyQt6_3D-6.6.0/sip/Qt3DExtras/qplanegeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1827 2023-10-25 10:21:13.719608 PyQt6_3D-6.6.0/sip/Qt3DExtras/qplanemesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1813 2023-10-25 10:21:13.735948 PyQt6_3D-6.6.0/sip/Qt3DExtras/qskyboxentity.sip
--rw-r--r--   0 phil       (501) staff       (20)     2106 2023-10-25 10:21:13.737836 PyQt6_3D-6.6.0/sip/Qt3DExtras/qspheregeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1794 2023-10-25 10:21:13.720886 PyQt6_3D-6.6.0/sip/Qt3DExtras/qspheregeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1752 2023-10-25 10:21:13.725178 PyQt6_3D-6.6.0/sip/Qt3DExtras/qspheremesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1501 2023-10-25 10:21:13.728009 PyQt6_3D-6.6.0/sip/Qt3DExtras/qspritegrid.sip
--rw-r--r--   0 phil       (501) staff       (20)     1739 2023-10-25 10:21:13.726294 PyQt6_3D-6.6.0/sip/Qt3DExtras/qspritesheet.sip
--rw-r--r--   0 phil       (501) staff       (20)     1635 2023-10-25 10:21:13.726912 PyQt6_3D-6.6.0/sip/Qt3DExtras/qspritesheetitem.sip
--rw-r--r--   0 phil       (501) staff       (20)     7090 2023-10-25 10:21:13.731372 PyQt6_3D-6.6.0/sip/Qt3DExtras/qt3dwindow.sip
--rw-r--r--   0 phil       (501) staff       (20)     1847 2023-10-25 10:21:13.736510 PyQt6_3D-6.6.0/sip/Qt3DExtras/qtext2dentity.sip
--rw-r--r--   0 phil       (501) staff       (20)     2009 2023-10-25 10:21:13.724603 PyQt6_3D-6.6.0/sip/Qt3DExtras/qtexturematerial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2035 2023-10-25 10:21:13.723416 PyQt6_3D-6.6.0/sip/Qt3DExtras/qtorusgeometry.sip
--rw-r--r--   0 phil       (501) staff       (20)     1779 2023-10-25 10:21:13.729822 PyQt6_3D-6.6.0/sip/Qt3DExtras/qtorusgeometryview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1737 2023-10-25 10:21:13.731942 PyQt6_3D-6.6.0/sip/Qt3DExtras/qtorusmesh.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.140021 PyQt6_3D-6.6.0/sip/Qt3DInput/
--rw-r--r--   0 phil       (501) staff       (20)     2590 2023-10-25 10:21:13.698467 PyQt6_3D-6.6.0/sip/Qt3DInput/Qt3DInputmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1234 2023-10-25 10:21:13.704470 PyQt6_3D-6.6.0/sip/Qt3DInput/qabstractactioninput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1506 2023-10-25 10:21:13.710494 PyQt6_3D-6.6.0/sip/Qt3DInput/qabstractaxisinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     4384 2023-10-25 10:21:13.700673 PyQt6_3D-6.6.0/sip/Qt3DInput/qabstractphysicaldevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1742 2023-10-25 10:21:13.701310 PyQt6_3D-6.6.0/sip/Qt3DInput/qaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     1694 2023-10-25 10:21:13.705814 PyQt6_3D-6.6.0/sip/Qt3DInput/qactioninput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1417 2023-10-25 10:21:13.702574 PyQt6_3D-6.6.0/sip/Qt3DInput/qanalogaxisinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2023-10-25 10:21:13.699101 PyQt6_3D-6.6.0/sip/Qt3DInput/qaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2101 2023-10-25 10:21:13.701971 PyQt6_3D-6.6.0/sip/Qt3DInput/qaxisaccumulator.sip
--rw-r--r--   0 phil       (501) staff       (20)     1688 2023-10-25 10:21:13.696606 PyQt6_3D-6.6.0/sip/Qt3DInput/qaxissetting.sip
--rw-r--r--   0 phil       (501) staff       (20)     1852 2023-10-25 10:21:13.709059 PyQt6_3D-6.6.0/sip/Qt3DInput/qbuttonaxisinput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1405 2023-10-25 10:21:13.697821 PyQt6_3D-6.6.0/sip/Qt3DInput/qinputaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1836 2023-10-25 10:21:13.707159 PyQt6_3D-6.6.0/sip/Qt3DInput/qinputchord.sip
--rw-r--r--   0 phil       (501) staff       (20)     2010 2023-10-25 10:21:13.706497 PyQt6_3D-6.6.0/sip/Qt3DInput/qinputsequence.sip
--rw-r--r--   0 phil       (501) staff       (20)     1435 2023-10-25 10:21:13.703137 PyQt6_3D-6.6.0/sip/Qt3DInput/qinputsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1795 2023-10-25 10:21:13.708428 PyQt6_3D-6.6.0/sip/Qt3DInput/qkeyboarddevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     3906 2023-10-25 10:21:13.703921 PyQt6_3D-6.6.0/sip/Qt3DInput/qkeyboardhandler.sip
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-10-25 10:21:13.697243 PyQt6_3D-6.6.0/sip/Qt3DInput/qkeyevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2048 2023-10-25 10:21:13.707826 PyQt6_3D-6.6.0/sip/Qt3DInput/qlogicaldevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2065 2023-10-25 10:21:13.699791 PyQt6_3D-6.6.0/sip/Qt3DInput/qmousedevice.sip
--rw-r--r--   0 phil       (501) staff       (20)     2756 2023-10-25 10:21:13.709924 PyQt6_3D-6.6.0/sip/Qt3DInput/qmouseevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     2037 2023-10-25 10:21:13.705175 PyQt6_3D-6.6.0/sip/Qt3DInput/qmousehandler.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.141280 PyQt6_3D-6.6.0/sip/Qt3DLogic/
--rw-r--r--   0 phil       (501) staff       (20)     2006 2023-10-25 10:21:13.711160 PyQt6_3D-6.6.0/sip/Qt3DLogic/Qt3DLogicmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     2049 2023-10-25 10:21:13.711892 PyQt6_3D-6.6.0/sip/Qt3DLogic/qframeaction.sip
--rw-r--r--   0 phil       (501) staff       (20)     1254 2023-10-25 10:21:13.712431 PyQt6_3D-6.6.0/sip/Qt3DLogic/qlogicaspect.sip
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:21:14.207031 PyQt6_3D-6.6.0/sip/Qt3DRender/
--rw-r--r--   0 phil       (501) staff       (20)     4863 2023-10-25 10:21:13.816324 PyQt6_3D-6.6.0/sip/Qt3DRender/Qt3DRendermod.sip
--rw-r--r--   0 phil       (501) staff       (20)     1664 2023-10-25 10:21:13.789538 PyQt6_3D-6.6.0/sip/Qt3DRender/qabstractlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     2656 2023-10-25 10:21:13.809463 PyQt6_3D-6.6.0/sip/Qt3DRender/qabstractraycaster.sip
--rw-r--r--   0 phil       (501) staff       (20)     8855 2023-10-25 10:21:13.788392 PyQt6_3D-6.6.0/sip/Qt3DRender/qabstracttexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     1933 2023-10-25 10:21:13.794795 PyQt6_3D-6.6.0/sip/Qt3DRender/qabstracttextureimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1275 2023-10-25 10:21:13.791693 PyQt6_3D-6.6.0/sip/Qt3DRender/qalphacoverage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1915 2023-10-25 10:21:13.812949 PyQt6_3D-6.6.0/sip/Qt3DRender/qalphatest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1731 2023-10-25 10:21:13.777980 PyQt6_3D-6.6.0/sip/Qt3DRender/qblendequation.sip
--rw-r--r--   0 phil       (501) staff       (20)     3658 2023-10-25 10:21:13.782488 PyQt6_3D-6.6.0/sip/Qt3DRender/qblendequationarguments.sip
--rw-r--r--   0 phil       (501) staff       (20)     2712 2023-10-25 10:21:13.810002 PyQt6_3D-6.6.0/sip/Qt3DRender/qblitframebuffer.sip
--rw-r--r--   0 phil       (501) staff       (20)    15325 2023-10-25 10:21:13.770234 PyQt6_3D-6.6.0/sip/Qt3DRender/qcamera.sip
--rw-r--r--   0 phil       (501) staff       (20)     3588 2023-10-25 10:21:13.815453 PyQt6_3D-6.6.0/sip/Qt3DRender/qcameralens.sip
--rw-r--r--   0 phil       (501) staff       (20)     1466 2023-10-25 10:21:13.774002 PyQt6_3D-6.6.0/sip/Qt3DRender/qcameraselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     2555 2023-10-25 10:21:13.772933 PyQt6_3D-6.6.0/sip/Qt3DRender/qclearbuffers.sip
--rw-r--r--   0 phil       (501) staff       (20)     1623 2023-10-25 10:21:13.784251 PyQt6_3D-6.6.0/sip/Qt3DRender/qclipplane.sip
--rw-r--r--   0 phil       (501) staff       (20)     1805 2023-10-25 10:21:13.808830 PyQt6_3D-6.6.0/sip/Qt3DRender/qcolormask.sip
--rw-r--r--   0 phil       (501) staff       (20)     2069 2023-10-25 10:21:13.760908 PyQt6_3D-6.6.0/sip/Qt3DRender/qcomputecommand.sip
--rw-r--r--   0 phil       (501) staff       (20)     1617 2023-10-25 10:21:13.792632 PyQt6_3D-6.6.0/sip/Qt3DRender/qcullface.sip
--rw-r--r--   0 phil       (501) staff       (20)     1534 2023-10-25 10:21:13.808288 PyQt6_3D-6.6.0/sip/Qt3DRender/qdepthrange.sip
--rw-r--r--   0 phil       (501) staff       (20)     1765 2023-10-25 10:21:13.804700 PyQt6_3D-6.6.0/sip/Qt3DRender/qdepthtest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1504 2023-10-25 10:21:13.792147 PyQt6_3D-6.6.0/sip/Qt3DRender/qdirectionallight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1653 2023-10-25 10:21:13.796437 PyQt6_3D-6.6.0/sip/Qt3DRender/qdispatchcompute.sip
--rw-r--r--   0 phil       (501) staff       (20)     1251 2023-10-25 10:21:13.791210 PyQt6_3D-6.6.0/sip/Qt3DRender/qdithering.sip
--rw-r--r--   0 phil       (501) staff       (20)     2066 2023-10-25 10:21:13.817955 PyQt6_3D-6.6.0/sip/Qt3DRender/qeffect.sip
--rw-r--r--   0 phil       (501) staff       (20)     1770 2023-10-25 10:21:13.793148 PyQt6_3D-6.6.0/sip/Qt3DRender/qenvironmentlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1529 2023-10-25 10:21:13.776672 PyQt6_3D-6.6.0/sip/Qt3DRender/qfilterkey.sip
--rw-r--r--   0 phil       (501) staff       (20)     1339 2023-10-25 10:21:13.816784 PyQt6_3D-6.6.0/sip/Qt3DRender/qframegraphnode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1638 2023-10-25 10:21:13.814290 PyQt6_3D-6.6.0/sip/Qt3DRender/qfrontface.sip
--rw-r--r--   0 phil       (501) staff       (20)     1284 2023-10-25 10:21:13.802961 PyQt6_3D-6.6.0/sip/Qt3DRender/qfrustumculling.sip
--rw-r--r--   0 phil       (501) staff       (20)     3665 2023-10-25 10:21:13.790779 PyQt6_3D-6.6.0/sip/Qt3DRender/qgeometryrenderer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2598 2023-10-25 10:21:13.760385 PyQt6_3D-6.6.0/sip/Qt3DRender/qgraphicsapifilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1345 2023-10-25 10:21:13.768824 PyQt6_3D-6.6.0/sip/Qt3DRender/qlayer.sip
--rw-r--r--   0 phil       (501) staff       (20)     2112 2023-10-25 10:21:13.795910 PyQt6_3D-6.6.0/sip/Qt3DRender/qlayerfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2582 2023-10-25 10:21:13.770883 PyQt6_3D-6.6.0/sip/Qt3DRender/qlevelofdetail.sip
--rw-r--r--   0 phil       (501) staff       (20)     1682 2023-10-25 10:21:13.802099 PyQt6_3D-6.6.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip
--rw-r--r--   0 phil       (501) staff       (20)     1313 2023-10-25 10:21:13.807820 PyQt6_3D-6.6.0/sip/Qt3DRender/qlevelofdetailswitch.sip
--rw-r--r--   0 phil       (501) staff       (20)     1498 2023-10-25 10:21:13.766316 PyQt6_3D-6.6.0/sip/Qt3DRender/qlinewidth.sip
--rw-r--r--   0 phil       (501) staff       (20)     7581 2023-10-25 10:21:13.812359 PyQt6_3D-6.6.0/sip/Qt3DRender/qlist.sip
--rw-r--r--   0 phil       (501) staff       (20)     1635 2023-10-25 10:21:13.800074 PyQt6_3D-6.6.0/sip/Qt3DRender/qmaterial.sip
--rw-r--r--   0 phil       (501) staff       (20)     2100 2023-10-25 10:21:13.817324 PyQt6_3D-6.6.0/sip/Qt3DRender/qmemorybarrier.sip
--rw-r--r--   0 phil       (501) staff       (20)     1797 2023-10-25 10:21:13.779064 PyQt6_3D-6.6.0/sip/Qt3DRender/qmesh.sip
--rw-r--r--   0 phil       (501) staff       (20)     1335 2023-10-25 10:21:13.785328 PyQt6_3D-6.6.0/sip/Qt3DRender/qmultisampleantialiasing.sip
--rw-r--r--   0 phil       (501) staff       (20)     1263 2023-10-25 10:21:13.798000 PyQt6_3D-6.6.0/sip/Qt3DRender/qnodepthmask.sip
--rw-r--r--   0 phil       (501) staff       (20)     1236 2023-10-25 10:21:13.813367 PyQt6_3D-6.6.0/sip/Qt3DRender/qnodraw.sip
--rw-r--r--   0 phil       (501) staff       (20)     1254 2023-10-25 10:21:13.802526 PyQt6_3D-6.6.0/sip/Qt3DRender/qnopicking.sip
--rw-r--r--   0 phil       (501) staff       (20)     2105 2023-10-25 10:21:13.768368 PyQt6_3D-6.6.0/sip/Qt3DRender/qobjectpicker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1850 2023-10-25 10:21:13.767241 PyQt6_3D-6.6.0/sip/Qt3DRender/qpaintedtextureimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     1752 2023-10-25 10:21:13.763284 PyQt6_3D-6.6.0/sip/Qt3DRender/qparameter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2414 2023-10-25 10:21:13.805466 PyQt6_3D-6.6.0/sip/Qt3DRender/qpickevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1270 2023-10-25 10:21:13.761318 PyQt6_3D-6.6.0/sip/Qt3DRender/qpickingproxy.sip
--rw-r--r--   0 phil       (501) staff       (20)     2955 2023-10-25 10:21:13.759705 PyQt6_3D-6.6.0/sip/Qt3DRender/qpickingsettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1583 2023-10-25 10:21:13.773547 PyQt6_3D-6.6.0/sip/Qt3DRender/qpicklineevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1484 2023-10-25 10:21:13.774998 PyQt6_3D-6.6.0/sip/Qt3DRender/qpickpointevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1944 2023-10-25 10:21:13.803553 PyQt6_3D-6.6.0/sip/Qt3DRender/qpicktriangleevent.sip
--rw-r--r--   0 phil       (501) staff       (20)     1771 2023-10-25 10:21:13.805960 PyQt6_3D-6.6.0/sip/Qt3DRender/qpointlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1698 2023-10-25 10:21:13.781834 PyQt6_3D-6.6.0/sip/Qt3DRender/qpointsize.sip
--rw-r--r--   0 phil       (501) staff       (20)     1573 2023-10-25 10:21:13.782964 PyQt6_3D-6.6.0/sip/Qt3DRender/qpolygonoffset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1637 2023-10-25 10:21:13.785877 PyQt6_3D-6.6.0/sip/Qt3DRender/qproximityfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     1924 2023-10-25 10:21:13.804171 PyQt6_3D-6.6.0/sip/Qt3DRender/qrastermode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1800 2023-10-25 10:21:13.801499 PyQt6_3D-6.6.0/sip/Qt3DRender/qraycaster.sip
--rw-r--r--   0 phil       (501) staff       (20)     2004 2023-10-25 10:21:13.761937 PyQt6_3D-6.6.0/sip/Qt3DRender/qraycasterhit.sip
--rw-r--r--   0 phil       (501) staff       (20)     1151 2023-10-25 10:21:13.786359 PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderapi.sip
--rw-r--r--   0 phil       (501) staff       (20)     1555 2023-10-25 10:21:13.764866 PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderaspect.sip
--rw-r--r--   0 phil       (501) staff       (20)     2740 2023-10-25 10:21:13.783758 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendercapabilities.sip
--rw-r--r--   0 phil       (501) staff       (20)     1846 2023-10-25 10:21:13.810497 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendercapture.sip
--rw-r--r--   0 phil       (501) staff       (20)     2788 2023-10-25 10:21:13.795392 PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderpass.sip
--rw-r--r--   0 phil       (501) staff       (20)     2140 2023-10-25 10:21:13.772337 PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderpassfilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     2036 2023-10-25 10:21:13.798501 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendersettings.sip
--rw-r--r--   0 phil       (501) staff       (20)     1196 2023-10-25 10:21:13.800500 PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderstate.sip
--rw-r--r--   0 phil       (501) staff       (20)     1719 2023-10-25 10:21:13.814746 PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderstateset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1804 2023-10-25 10:21:13.775926 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendersurfaceselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     1703 2023-10-25 10:21:13.813825 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendertarget.sip
--rw-r--r--   0 phil       (501) staff       (20)     2734 2023-10-25 10:21:13.806772 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendertargetoutput.sip
--rw-r--r--   0 phil       (501) staff       (20)     1545 2023-10-25 10:21:13.766753 PyQt6_3D-6.6.0/sip/Qt3DRender/qrendertargetselector.sip
--rw-r--r--   0 phil       (501) staff       (20)     2168 2023-10-25 10:21:13.786901 PyQt6_3D-6.6.0/sip/Qt3DRender/qsceneloader.sip
--rw-r--r--   0 phil       (501) staff       (20)     1697 2023-10-25 10:21:13.757089 PyQt6_3D-6.6.0/sip/Qt3DRender/qscissortest.sip
--rw-r--r--   0 phil       (501) staff       (20)     1533 2023-10-25 10:21:13.777321 PyQt6_3D-6.6.0/sip/Qt3DRender/qscreenraycaster.sip
--rw-r--r--   0 phil       (501) staff       (20)     1287 2023-10-25 10:21:13.784845 PyQt6_3D-6.6.0/sip/Qt3DRender/qseamlesscubemap.sip
--rw-r--r--   0 phil       (501) staff       (20)     1575 2023-10-25 10:21:13.788912 PyQt6_3D-6.6.0/sip/Qt3DRender/qsetfence.sip
--rw-r--r--   0 phil       (501) staff       (20)     1690 2023-10-25 10:21:13.762411 PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderdata.sip
--rw-r--r--   0 phil       (501) staff       (20)     3207 2023-10-25 10:21:13.758475 PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     3718 2023-10-25 10:21:13.771707 PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderprogram.sip
--rw-r--r--   0 phil       (501) staff       (20)     3778 2023-10-25 10:21:13.757775 PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderprogrambuilder.sip
--rw-r--r--   0 phil       (501) staff       (20)     1904 2023-10-25 10:21:13.796950 PyQt6_3D-6.6.0/sip/Qt3DRender/qsortpolicy.sip
--rw-r--r--   0 phil       (501) staff       (20)     2076 2023-10-25 10:21:13.764409 PyQt6_3D-6.6.0/sip/Qt3DRender/qspotlight.sip
--rw-r--r--   0 phil       (501) staff       (20)     1595 2023-10-25 10:21:13.807246 PyQt6_3D-6.6.0/sip/Qt3DRender/qstencilmask.sip
--rw-r--r--   0 phil       (501) staff       (20)     1418 2023-10-25 10:21:13.765277 PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciloperation.sip
--rw-r--r--   0 phil       (501) staff       (20)     2778 2023-10-25 10:21:13.767826 PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciloperationarguments.sip
--rw-r--r--   0 phil       (501) staff       (20)     1378 2023-10-25 10:21:13.801017 PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciltest.sip
--rw-r--r--   0 phil       (501) staff       (20)     2409 2023-10-25 10:21:13.799098 PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciltestarguments.sip
--rw-r--r--   0 phil       (501) staff       (20)     1655 2023-10-25 10:21:13.765869 PyQt6_3D-6.6.0/sip/Qt3DRender/qsubtreeenabler.sip
--rw-r--r--   0 phil       (501) staff       (20)     2572 2023-10-25 10:21:13.797505 PyQt6_3D-6.6.0/sip/Qt3DRender/qtechnique.sip
--rw-r--r--   0 phil       (501) staff       (20)     2118 2023-10-25 10:21:13.780259 PyQt6_3D-6.6.0/sip/Qt3DRender/qtechniquefilter.sip
--rw-r--r--   0 phil       (501) staff       (20)     4644 2023-10-25 10:21:13.794277 PyQt6_3D-6.6.0/sip/Qt3DRender/qtexture.sip
--rw-r--r--   0 phil       (501) staff       (20)     3172 2023-10-25 10:21:13.779738 PyQt6_3D-6.6.0/sip/Qt3DRender/qtexturedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     2108 2023-10-25 10:21:13.763882 PyQt6_3D-6.6.0/sip/Qt3DRender/qtexturedataupdate.sip
--rw-r--r--   0 phil       (501) staff       (20)     2041 2023-10-25 10:21:13.759094 PyQt6_3D-6.6.0/sip/Qt3DRender/qtextureimage.sip
--rw-r--r--   0 phil       (501) staff       (20)     2474 2023-10-25 10:21:13.790079 PyQt6_3D-6.6.0/sip/Qt3DRender/qtextureimagedata.sip
--rw-r--r--   0 phil       (501) staff       (20)     1539 2023-10-25 10:21:13.762832 PyQt6_3D-6.6.0/sip/Qt3DRender/qtextureimagedatagenerator.sip
--rw-r--r--   0 phil       (501) staff       (20)     2330 2023-10-25 10:21:13.781120 PyQt6_3D-6.6.0/sip/Qt3DRender/qtexturewrapmode.sip
--rw-r--r--   0 phil       (501) staff       (20)     1599 2023-10-25 10:21:13.799604 PyQt6_3D-6.6.0/sip/Qt3DRender/qviewport.sip
--rw-r--r--   0 phil       (501) staff       (20)     1943 2023-10-25 10:21:13.774499 PyQt6_3D-6.6.0/sip/Qt3DRender/qwaitfence.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.385180 PyQt6_3D-6.7.0/
+-rw-r--r--   0 phil       (501) staff       (20)    11024 2024-04-20 16:00:59.953136 PyQt6_3D-6.7.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2024-04-20 16:00:59.855068 PyQt6_3D-6.7.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      744 2024-04-20 15:58:18.805801 PyQt6_3D-6.7.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1533 2024-04-20 16:01:00.385249 PyQt6_3D-6.7.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1174 2024-04-20 16:00:59.953764 PyQt6_3D-6.7.0/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.326244 PyQt6_3D-6.7.0/examples/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.337863 PyQt6_3D-6.7.0/examples/assets/
+-rw-r--r--   0 phil       (501) staff       (20)      136 2024-04-20 15:58:18.810794 PyQt6_3D-6.7.0/examples/assets/LICENSE
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.337674 PyQt6_3D-6.7.0/examples/assets/chest/
+-rw-r--r--   0 phil       (501) staff       (20)    46344 2024-04-20 15:58:18.811334 PyQt6_3D-6.7.0/examples/assets/chest/Chest.obj
+-rw-r--r--   0 phil       (501) staff       (20)    70980 2024-04-20 15:58:18.811894 PyQt6_3D-6.7.0/examples/assets/chest/diffuse.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.330456 PyQt6_3D-6.7.0/examples/assets/cubemaps/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.330281 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/
+-rw-r--r--   0 phil       (501) staff       (20)      293 2024-04-20 15:58:18.812254 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/README.TXT
+-rw-r--r--   0 phil       (501) staff       (20)   121754 2024-04-20 15:58:18.812989 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_negx.webp
+-rw-r--r--   0 phil       (501) staff       (20)     1926 2024-04-20 15:58:18.813247 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_negy.webp
+-rw-r--r--   0 phil       (501) staff       (20)   147696 2024-04-20 15:58:18.814087 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_negz.webp
+-rw-r--r--   0 phil       (501) staff       (20)   136426 2024-04-20 15:58:18.814867 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_posx.webp
+-rw-r--r--   0 phil       (501) staff       (20)    57622 2024-04-20 15:58:18.815319 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_posy.webp
+-rw-r--r--   0 phil       (501) staff       (20)   164564 2024-04-20 15:58:18.816133 PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_posz.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.331396 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/
+-rw-r--r--   0 phil       (501) staff       (20)    38042 2024-04-20 15:58:18.816581 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_negx.webp
+-rw-r--r--   0 phil       (501) staff       (20)    42278 2024-04-20 15:58:18.817002 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_negy.webp
+-rw-r--r--   0 phil       (501) staff       (20)    36790 2024-04-20 15:58:18.817373 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_negz.webp
+-rw-r--r--   0 phil       (501) staff       (20)    37092 2024-04-20 15:58:18.817743 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_posx.webp
+-rw-r--r--   0 phil       (501) staff       (20)    26008 2024-04-20 15:58:18.818133 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_posy.webp
+-rw-r--r--   0 phil       (501) staff       (20)    37802 2024-04-20 15:58:18.818543 PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_posz.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.331783 PyQt6_3D-6.7.0/examples/assets/gltf/
+-rw-r--r--   0 phil       (501) staff       (20)     1831 2024-04-20 15:58:18.818772 PyQt6_3D-6.7.0/examples/assets/gltf/LICENSE.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.334354 PyQt6_3D-6.7.0/examples/assets/gltf/wine/
+-rw-r--r--   0 phil       (501) staff       (20)     8798 2024-04-20 15:58:18.819128 PyQt6_3D-6.7.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg
+-rw-r--r--   0 phil       (501) staff       (20)    46051 2024-04-20 15:58:18.819665 PyQt6_3D-6.7.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg
+-rw-r--r--   0 phil       (501) staff       (20)    35585 2024-04-20 15:58:18.820136 PyQt6_3D-6.7.0/examples/assets/gltf/wine/artezin_bottle.jpg
+-rw-r--r--   0 phil       (501) staff       (20)   329088 2024-04-20 15:58:18.821566 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine.bin
+-rw-r--r--   0 phil       (501) staff       (20)   797366 2024-04-20 15:58:18.824345 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine.dae
+-rw-r--r--   0 phil       (501) staff       (20)   275432 2024-04-20 15:58:18.825374 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine.gltf
+-rw-r--r--   0 phil       (501) staff       (20)      497 2024-04-20 15:58:18.825581 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine0FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      439 2024-04-20 15:58:18.825772 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine0VS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      489 2024-04-20 15:58:18.825954 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine1FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      355 2024-04-20 15:58:18.826138 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine1VS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      219 2024-04-20 15:58:18.826323 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine2FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      236 2024-04-20 15:58:18.826506 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine2VS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      441 2024-04-20 15:58:18.826685 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine3FS.glsl
+-rw-r--r--   0 phil       (501) staff       (20)      355 2024-04-20 15:58:18.826862 PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine3VS.glsl
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.346334 PyQt6_3D-6.7.0/examples/assets/houseplants/
+-rw-r--r--   0 phil       (501) staff       (20)    13846 2024-04-20 15:58:18.827258 PyQt6_3D-6.7.0/examples/assets/houseplants/bamboo.webp
+-rw-r--r--   0 phil       (501) staff       (20)    16614 2024-04-20 15:58:18.827535 PyQt6_3D-6.7.0/examples/assets/houseplants/bamboo_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    89192 2024-04-20 15:58:18.828102 PyQt6_3D-6.7.0/examples/assets/houseplants/cover.webp
+-rw-r--r--   0 phil       (501) staff       (20)    21098 2024-04-20 15:58:18.828455 PyQt6_3D-6.7.0/examples/assets/houseplants/cover_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    44264 2024-04-20 15:58:18.828856 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36076 2024-04-20 15:58:18.829306 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9324 2024-04-20 15:58:18.829531 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1822 2024-04-20 15:58:18.829713 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     8863 2024-04-20 15:58:18.829930 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15838 2024-04-20 15:58:18.830283 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2216 2024-04-20 15:58:18.830462 PyQt6_3D-6.7.0/examples/assets/houseplants/cross-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    51505 2024-04-20 15:58:18.830834 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36078 2024-04-20 15:58:18.831145 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2024-04-20 15:58:18.831371 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1820 2024-04-20 15:58:18.831558 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9026 2024-04-20 15:58:18.831776 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2024-04-20 15:58:18.832138 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2216 2024-04-20 15:58:18.832435 PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    33756 2024-04-20 15:58:18.832698 PyQt6_3D-6.7.0/examples/assets/houseplants/palm.webp
+-rw-r--r--   0 phil       (501) staff       (20)    36186 2024-04-20 15:58:18.832973 PyQt6_3D-6.7.0/examples/assets/houseplants/palm_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)   120426 2024-04-20 15:58:18.833464 PyQt6_3D-6.7.0/examples/assets/houseplants/pine.webp
+-rw-r--r--   0 phil       (501) staff       (20)    47352 2024-04-20 15:58:18.833770 PyQt6_3D-6.7.0/examples/assets/houseplants/pine_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)   366144 2024-04-20 15:58:18.835090 PyQt6_3D-6.7.0/examples/assets/houseplants/pot.webp
+-rw-r--r--   0 phil       (501) staff       (20)    50950 2024-04-20 15:58:18.835537 PyQt6_3D-6.7.0/examples/assets/houseplants/pot_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    33100 2024-04-20 15:58:18.835893 PyQt6_3D-6.7.0/examples/assets/houseplants/shrub.webp
+-rw-r--r--   0 phil       (501) staff       (20)    10180 2024-04-20 15:58:18.836176 PyQt6_3D-6.7.0/examples/assets/houseplants/shrub_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    51509 2024-04-20 15:58:18.837962 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36082 2024-04-20 15:58:18.838327 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2024-04-20 15:58:18.838580 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1820 2024-04-20 15:58:18.838772 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)    46455 2024-04-20 15:58:18.839440 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2024-04-20 15:58:18.839706 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2220 2024-04-20 15:58:18.839902 PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    30338 2024-04-20 15:58:18.840252 PyQt6_3D-6.7.0/examples/assets/houseplants/spikes.webp
+-rw-r--r--   0 phil       (501) staff       (20)    12028 2024-04-20 15:58:18.840546 PyQt6_3D-6.7.0/examples/assets/houseplants/spikes_normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)    51509 2024-04-20 15:58:18.840964 PyQt6_3D-6.7.0/examples/assets/houseplants/square-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36082 2024-04-20 15:58:18.841296 PyQt6_3D-6.7.0/examples/assets/houseplants/square-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2024-04-20 15:58:18.841525 PyQt6_3D-6.7.0/examples/assets/houseplants/square-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1824 2024-04-20 15:58:18.841721 PyQt6_3D-6.7.0/examples/assets/houseplants/square-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     3725 2024-04-20 15:58:18.841917 PyQt6_3D-6.7.0/examples/assets/houseplants/square-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2024-04-20 15:58:18.842173 PyQt6_3D-6.7.0/examples/assets/houseplants/square-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2220 2024-04-20 15:58:18.842359 PyQt6_3D-6.7.0/examples/assets/houseplants/square-spikes.obj
+-rw-r--r--   0 phil       (501) staff       (20)    28687 2024-04-20 15:58:18.842700 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-bamboo.obj
+-rw-r--r--   0 phil       (501) staff       (20)    36082 2024-04-20 15:58:18.843011 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-palm.obj
+-rw-r--r--   0 phil       (501) staff       (20)     9328 2024-04-20 15:58:18.843254 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-pine.obj
+-rw-r--r--   0 phil       (501) staff       (20)     1808 2024-04-20 15:58:18.843446 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-pot-cover.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2469 2024-04-20 15:58:18.843631 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-pot.obj
+-rw-r--r--   0 phil       (501) staff       (20)    15842 2024-04-20 15:58:18.843888 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-shrub.obj
+-rw-r--r--   0 phil       (501) staff       (20)     2220 2024-04-20 15:58:18.844075 PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-spikes.obj
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.337259 PyQt6_3D-6.7.0/examples/assets/metalbarrel/
+-rw-r--r--   0 phil       (501) staff       (20)   162040 2024-04-20 15:58:18.844938 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_black.webp
+-rw-r--r--   0 phil       (501) staff       (20)   101158 2024-04-20 15:58:18.845543 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_blue.webp
+-rw-r--r--   0 phil       (501) staff       (20)    74498 2024-04-20 15:58:18.846055 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_green.webp
+-rw-r--r--   0 phil       (501) staff       (20)    86874 2024-04-20 15:58:18.846574 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_red.webp
+-rw-r--r--   0 phil       (501) staff       (20)   254934 2024-04-20 15:58:18.847611 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_rust.webp
+-rw-r--r--   0 phil       (501) staff       (20)     6042 2024-04-20 15:58:18.847844 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_stainless_steel.webp
+-rw-r--r--   0 phil       (501) staff       (20)   101134 2024-04-20 15:58:18.848423 PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_yellow.webp
+-rw-r--r--   0 phil       (501) staff       (20)    27126 2024-04-20 15:58:18.848702 PyQt6_3D-6.7.0/examples/assets/metalbarrel/metal_barrel.obj
+-rw-r--r--   0 phil       (501) staff       (20)    29446 2024-04-20 15:58:18.849095 PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_hard_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)    25560 2024-04-20 15:58:18.849470 PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_middle_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)    21544 2024-04-20 15:58:18.849743 PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_no_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)    23620 2024-04-20 15:58:18.850018 PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_soft_bumps.webp
+-rw-r--r--   0 phil       (501) staff       (20)   420416 2024-04-20 15:58:18.851394 PyQt6_3D-6.7.0/examples/assets/metalbarrel/specular.webp
+-rw-r--r--   0 phil       (501) staff       (20)   330298 2024-04-20 15:58:18.852533 PyQt6_3D-6.7.0/examples/assets/metalbarrel/specular_rust.webp
+-rw-r--r--   0 phil       (501) staff       (20)   220224 2024-04-20 15:58:18.853534 PyQt6_3D-6.7.0/examples/assets/metalbarrel/specular_stainless_steel.webp
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.327444 PyQt6_3D-6.7.0/examples/assets/obj/
+-rw-r--r--   0 phil       (501) staff       (20)   346814 2024-04-20 15:58:18.854941 PyQt6_3D-6.7.0/examples/assets/obj/ball.obj
+-rw-r--r--   0 phil       (501) staff       (20)  1764501 2024-04-20 15:58:18.861020 PyQt6_3D-6.7.0/examples/assets/obj/toyplane.obj
+-rw-r--r--   0 phil       (501) staff       (20)   263373 2024-04-20 15:58:18.862438 PyQt6_3D-6.7.0/examples/assets/obj/trefoil.obj
+-rw-r--r--   0 phil       (501) staff       (20)   127711 2024-04-20 15:58:18.863169 PyQt6_3D-6.7.0/examples/assets/test_scene.dae
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.327697 PyQt6_3D-6.7.0/examples/assets/textures/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.328620 PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/
+-rw-r--r--   0 phil       (501) staff       (20)   677322 2024-04-20 15:58:18.866696 PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/diffuse.webp
+-rw-r--r--   0 phil       (501) staff       (20)   822594 2024-04-20 15:58:18.869183 PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/normal.webp
+-rw-r--r--   0 phil       (501) staff       (20)      152 2024-04-20 15:58:18.869430 PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/readme.txt
+-rw-r--r--   0 phil       (501) staff       (20)  1005334 2024-04-20 15:58:18.872978 PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/specular.webp
+-rw-r--r--   0 phil       (501) staff       (20)    10285 2024-04-20 15:58:18.873293 PyQt6_3D-6.7.0/examples/basicshapes-py.py
+-rw-r--r--   0 phil       (501) staff       (20)    18568 2024-04-20 15:58:18.873560 PyQt6_3D-6.7.0/examples/materials-py.py
+-rw-r--r--   0 phil       (501) staff       (20)     6082 2024-04-20 15:58:18.873756 PyQt6_3D-6.7.0/examples/simple-py.py
+-rw-r--r--   0 phil       (501) staff       (20)     1040 2024-04-20 16:00:59.954007 PyQt6_3D-6.7.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.368545 PyQt6_3D-6.7.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.368332 PyQt6_3D-6.7.0/sip/Qt3DAnimation/
+-rw-r--r--   0 phil       (501) staff       (20)     2857 2024-04-20 16:01:00.170979 PyQt6_3D-6.7.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4851 2024-04-20 16:01:00.172181 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1351 2024-04-20 16:01:00.170680 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractanimationclip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1264 2024-04-20 16:01:00.164936 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractchannelmapping.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2221 2024-04-20 16:01:00.165561 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractclipanimator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1343 2024-04-20 16:01:00.171223 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractclipblendnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1966 2024-04-20 16:01:00.166772 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qadditiveclipblend.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1293 2024-04-20 16:01:00.167318 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1545 2024-04-20 16:01:00.169357 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationclip.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1631 2024-04-20 16:01:00.168132 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationclipdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1855 2024-04-20 16:01:00.165878 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationcliploader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2537 2024-04-20 16:01:00.168464 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationcontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1891 2024-04-20 16:01:00.164682 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationgroup.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1612 2024-04-20 16:01:00.165229 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qblendedclipanimator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1724 2024-04-20 16:01:00.169892 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannel.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1659 2024-04-20 16:01:00.166173 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannelcomponent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1504 2024-04-20 16:01:00.167576 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1765 2024-04-20 16:01:00.167061 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannelmapping.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1526 2024-04-20 16:01:00.170456 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qclipanimator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1653 2024-04-20 16:01:00.166481 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qclipblendvalue.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1388 2024-04-20 16:01:00.167854 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qclock.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2025 2024-04-20 16:01:00.171496 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qkeyframe.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2794 2024-04-20 16:01:00.170214 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qkeyframeanimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1907 2024-04-20 16:01:00.164374 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qlerpclipblend.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2786 2024-04-20 16:01:00.168815 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qmorphinganimation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1728 2024-04-20 16:01:00.169098 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qmorphtarget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1536 2024-04-20 16:01:00.171734 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qskeletonmapping.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2206 2024-04-20 16:01:00.169629 PyQt6_3D-6.7.0/sip/Qt3DAnimation/qvertexblendanimation.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.350463 PyQt6_3D-6.7.0/sip/Qt3DCore/
+-rw-r--r--   0 phil       (501) staff       (20)     2762 2024-04-20 16:01:00.141348 PyQt6_3D-6.7.0/sip/Qt3DCore/Qt3DCoremod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1564 2024-04-20 16:01:00.141591 PyQt6_3D-6.7.0/sip/Qt3DCore/qabstractaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1262 2024-04-20 16:01:00.138644 PyQt6_3D-6.7.0/sip/Qt3DCore/qabstractfunctor.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1318 2024-04-20 16:01:00.141833 PyQt6_3D-6.7.0/sip/Qt3DCore/qabstractskeleton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1466 2024-04-20 16:01:00.137620 PyQt6_3D-6.7.0/sip/Qt3DCore/qarmature.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2115 2024-04-20 16:01:00.138967 PyQt6_3D-6.7.0/sip/Qt3DCore/qaspectengine.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4242 2024-04-20 16:01:00.142259 PyQt6_3D-6.7.0/sip/Qt3DCore/qattribute.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2024 2024-04-20 16:01:00.143129 PyQt6_3D-6.7.0/sip/Qt3DCore/qbackendnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2131 2024-04-20 16:01:00.142822 PyQt6_3D-6.7.0/sip/Qt3DCore/qboundingvolume.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2259 2024-04-20 16:01:00.136910 PyQt6_3D-6.7.0/sip/Qt3DCore/qbuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1611 2024-04-20 16:01:00.139592 PyQt6_3D-6.7.0/sip/Qt3DCore/qcomponent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1488 2024-04-20 16:01:00.137900 PyQt6_3D-6.7.0/sip/Qt3DCore/qcoresettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1747 2024-04-20 16:01:00.139275 PyQt6_3D-6.7.0/sip/Qt3DCore/qentity.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2189 2024-04-20 16:01:00.140432 PyQt6_3D-6.7.0/sip/Qt3DCore/qgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3353 2024-04-20 16:01:00.137320 PyQt6_3D-6.7.0/sip/Qt3DCore/qgeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2581 2024-04-20 16:01:00.136525 PyQt6_3D-6.7.0/sip/Qt3DCore/qjoint.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4051 2024-04-20 16:01:00.138376 PyQt6_3D-6.7.0/sip/Qt3DCore/qnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1631 2024-04-20 16:01:00.142530 PyQt6_3D-6.7.0/sip/Qt3DCore/qnodeid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3247 2024-04-20 16:01:00.140137 PyQt6_3D-6.7.0/sip/Qt3DCore/qsharedpointer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1436 2024-04-20 16:01:00.140678 PyQt6_3D-6.7.0/sip/Qt3DCore/qskeleton.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2047 2024-04-20 16:01:00.143429 PyQt6_3D-6.7.0/sip/Qt3DCore/qskeletonloader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3357 2024-04-20 16:01:00.141026 PyQt6_3D-6.7.0/sip/Qt3DCore/qtransform.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.363612 PyQt6_3D-6.7.0/sip/Qt3DExtras/
+-rw-r--r--   0 phil       (501) staff       (20)     3472 2024-04-20 16:01:00.163050 PyQt6_3D-6.7.0/sip/Qt3DExtras/Qt3DExtrasmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2132 2024-04-20 16:01:00.155203 PyQt6_3D-6.7.0/sip/Qt3DExtras/qabstractcameracontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1716 2024-04-20 16:01:00.156542 PyQt6_3D-6.7.0/sip/Qt3DExtras/qabstractspritesheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2455 2024-04-20 16:01:00.152458 PyQt6_3D-6.7.0/sip/Qt3DExtras/qconegeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2199 2024-04-20 16:01:00.163384 PyQt6_3D-6.7.0/sip/Qt3DExtras/qconegeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2157 2024-04-20 16:01:00.151797 PyQt6_3D-6.7.0/sip/Qt3DExtras/qconemesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2505 2024-04-20 16:01:00.154079 PyQt6_3D-6.7.0/sip/Qt3DExtras/qcuboidgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2193 2024-04-20 16:01:00.155762 PyQt6_3D-6.7.0/sip/Qt3DExtras/qcuboidgeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2151 2024-04-20 16:01:00.163722 PyQt6_3D-6.7.0/sip/Qt3DExtras/qcuboidmesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2035 2024-04-20 16:01:00.153257 PyQt6_3D-6.7.0/sip/Qt3DExtras/qcylindergeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1779 2024-04-20 16:01:00.154620 PyQt6_3D-6.7.0/sip/Qt3DExtras/qcylindergeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1737 2024-04-20 16:01:00.164027 PyQt6_3D-6.7.0/sip/Qt3DExtras/qcylindermesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2077 2024-04-20 16:01:00.150815 PyQt6_3D-6.7.0/sip/Qt3DExtras/qdiffusemapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2198 2024-04-20 16:01:00.160564 PyQt6_3D-6.7.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2336 2024-04-20 16:01:00.151118 PyQt6_3D-6.7.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1887 2024-04-20 16:01:00.162310 PyQt6_3D-6.7.0/sip/Qt3DExtras/qextrudedtextgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1677 2024-04-20 16:01:00.161306 PyQt6_3D-6.7.0/sip/Qt3DExtras/qextrudedtextmesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1379 2024-04-20 16:01:00.160001 PyQt6_3D-6.7.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2854 2024-04-20 16:01:00.151497 PyQt6_3D-6.7.0/sip/Qt3DExtras/qforwardrenderer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2145 2024-04-20 16:01:00.154914 PyQt6_3D-6.7.0/sip/Qt3DExtras/qgoochmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2242 2024-04-20 16:01:00.158716 PyQt6_3D-6.7.0/sip/Qt3DExtras/qmetalroughmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2008 2024-04-20 16:01:00.157860 PyQt6_3D-6.7.0/sip/Qt3DExtras/qmorphphongmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1391 2024-04-20 16:01:00.152678 PyQt6_3D-6.7.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2313 2024-04-20 16:01:00.152968 PyQt6_3D-6.7.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2432 2024-04-20 16:01:00.158156 PyQt6_3D-6.7.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2785 2024-04-20 16:01:00.160998 PyQt6_3D-6.7.0/sip/Qt3DExtras/qorbitcameracontroller.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1333 2024-04-20 16:01:00.153484 PyQt6_3D-6.7.0/sip/Qt3DExtras/qpervertexcolormaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3397 2024-04-20 16:01:00.152143 PyQt6_3D-6.7.0/sip/Qt3DExtras/qphongalphamaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1838 2024-04-20 16:01:00.157334 PyQt6_3D-6.7.0/sip/Qt3DExtras/qphongmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2126 2024-04-20 16:01:00.159784 PyQt6_3D-6.7.0/sip/Qt3DExtras/qplanegeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1830 2024-04-20 16:01:00.160271 PyQt6_3D-6.7.0/sip/Qt3DExtras/qplanegeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1834 2024-04-20 16:01:00.153769 PyQt6_3D-6.7.0/sip/Qt3DExtras/qplanemesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1820 2024-04-20 16:01:00.161663 PyQt6_3D-6.7.0/sip/Qt3DExtras/qskyboxentity.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2113 2024-04-20 16:01:00.162644 PyQt6_3D-6.7.0/sip/Qt3DExtras/qspheregeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1801 2024-04-20 16:01:00.154343 PyQt6_3D-6.7.0/sip/Qt3DExtras/qspheregeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1759 2024-04-20 16:01:00.156298 PyQt6_3D-6.7.0/sip/Qt3DExtras/qspheremesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1508 2024-04-20 16:01:00.157579 PyQt6_3D-6.7.0/sip/Qt3DExtras/qspritegrid.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1746 2024-04-20 16:01:00.156799 PyQt6_3D-6.7.0/sip/Qt3DExtras/qspritesheet.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1642 2024-04-20 16:01:00.157067 PyQt6_3D-6.7.0/sip/Qt3DExtras/qspritesheetitem.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7097 2024-04-20 16:01:00.159214 PyQt6_3D-6.7.0/sip/Qt3DExtras/qt3dwindow.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1854 2024-04-20 16:01:00.161975 PyQt6_3D-6.7.0/sip/Qt3DExtras/qtext2dentity.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2016 2024-04-20 16:01:00.156030 PyQt6_3D-6.7.0/sip/Qt3DExtras/qtexturematerial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2042 2024-04-20 16:01:00.155486 PyQt6_3D-6.7.0/sip/Qt3DExtras/qtorusgeometry.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1786 2024-04-20 16:01:00.158436 PyQt6_3D-6.7.0/sip/Qt3DExtras/qtorusgeometryview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1744 2024-04-20 16:01:00.159498 PyQt6_3D-6.7.0/sip/Qt3DExtras/qtorusmesh.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.355577 PyQt6_3D-6.7.0/sip/Qt3DInput/
+-rw-r--r--   0 phil       (501) staff       (20)     2590 2024-04-20 16:01:00.144496 PyQt6_3D-6.7.0/sip/Qt3DInput/Qt3DInputmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1241 2024-04-20 16:01:00.147115 PyQt6_3D-6.7.0/sip/Qt3DInput/qabstractactioninput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1513 2024-04-20 16:01:00.149692 PyQt6_3D-6.7.0/sip/Qt3DInput/qabstractaxisinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4391 2024-04-20 16:01:00.145459 PyQt6_3D-6.7.0/sip/Qt3DInput/qabstractphysicaldevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1749 2024-04-20 16:01:00.145730 PyQt6_3D-6.7.0/sip/Qt3DInput/qaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1701 2024-04-20 16:01:00.147658 PyQt6_3D-6.7.0/sip/Qt3DInput/qactioninput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1424 2024-04-20 16:01:00.146267 PyQt6_3D-6.7.0/sip/Qt3DInput/qanalogaxisinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1726 2024-04-20 16:01:00.144762 PyQt6_3D-6.7.0/sip/Qt3DInput/qaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2108 2024-04-20 16:01:00.146031 PyQt6_3D-6.7.0/sip/Qt3DInput/qaxisaccumulator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1695 2024-04-20 16:01:00.143719 PyQt6_3D-6.7.0/sip/Qt3DInput/qaxissetting.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1859 2024-04-20 16:01:00.149028 PyQt6_3D-6.7.0/sip/Qt3DInput/qbuttonaxisinput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1412 2024-04-20 16:01:00.144209 PyQt6_3D-6.7.0/sip/Qt3DInput/qinputaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1843 2024-04-20 16:01:00.148214 PyQt6_3D-6.7.0/sip/Qt3DInput/qinputchord.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2017 2024-04-20 16:01:00.147942 PyQt6_3D-6.7.0/sip/Qt3DInput/qinputsequence.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1442 2024-04-20 16:01:00.146515 PyQt6_3D-6.7.0/sip/Qt3DInput/qinputsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1802 2024-04-20 16:01:00.148761 PyQt6_3D-6.7.0/sip/Qt3DInput/qkeyboarddevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3913 2024-04-20 16:01:00.146888 PyQt6_3D-6.7.0/sip/Qt3DInput/qkeyboardhandler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1722 2024-04-20 16:01:00.143985 PyQt6_3D-6.7.0/sip/Qt3DInput/qkeyevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2055 2024-04-20 16:01:00.148511 PyQt6_3D-6.7.0/sip/Qt3DInput/qlogicaldevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2072 2024-04-20 16:01:00.145052 PyQt6_3D-6.7.0/sip/Qt3DInput/qmousedevice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2770 2024-04-20 16:01:00.149448 PyQt6_3D-6.7.0/sip/Qt3DInput/qmouseevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2044 2024-04-20 16:01:00.147403 PyQt6_3D-6.7.0/sip/Qt3DInput/qmousehandler.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.356130 PyQt6_3D-6.7.0/sip/Qt3DLogic/
+-rw-r--r--   0 phil       (501) staff       (20)     2006 2024-04-20 16:01:00.149934 PyQt6_3D-6.7.0/sip/Qt3DLogic/Qt3DLogicmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2056 2024-04-20 16:01:00.150248 PyQt6_3D-6.7.0/sip/Qt3DLogic/qframeaction.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2024-04-20 16:01:00.150479 PyQt6_3D-6.7.0/sip/Qt3DLogic/qlogicaspect.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:00.385058 PyQt6_3D-6.7.0/sip/Qt3DRender/
+-rw-r--r--   0 phil       (501) staff       (20)     4863 2024-04-20 16:01:00.203621 PyQt6_3D-6.7.0/sip/Qt3DRender/Qt3DRendermod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1671 2024-04-20 16:01:00.189426 PyQt6_3D-6.7.0/sip/Qt3DRender/qabstractlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2663 2024-04-20 16:01:00.199713 PyQt6_3D-6.7.0/sip/Qt3DRender/qabstractraycaster.sip
+-rw-r--r--   0 phil       (501) staff       (20)     8862 2024-04-20 16:01:00.188858 PyQt6_3D-6.7.0/sip/Qt3DRender/qabstracttexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1940 2024-04-20 16:01:00.192313 PyQt6_3D-6.7.0/sip/Qt3DRender/qabstracttextureimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1282 2024-04-20 16:01:00.190620 PyQt6_3D-6.7.0/sip/Qt3DRender/qalphacoverage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1922 2024-04-20 16:01:00.201710 PyQt6_3D-6.7.0/sip/Qt3DRender/qalphatest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1738 2024-04-20 16:01:00.183328 PyQt6_3D-6.7.0/sip/Qt3DRender/qblendequation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3665 2024-04-20 16:01:00.185301 PyQt6_3D-6.7.0/sip/Qt3DRender/qblendequationarguments.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2719 2024-04-20 16:01:00.200020 PyQt6_3D-6.7.0/sip/Qt3DRender/qblitframebuffer.sip
+-rw-r--r--   0 phil       (501) staff       (20)    15332 2024-04-20 16:01:00.179945 PyQt6_3D-6.7.0/sip/Qt3DRender/qcamera.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3595 2024-04-20 16:01:00.203098 PyQt6_3D-6.7.0/sip/Qt3DRender/qcameralens.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1473 2024-04-20 16:01:00.181786 PyQt6_3D-6.7.0/sip/Qt3DRender/qcameraselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2562 2024-04-20 16:01:00.181316 PyQt6_3D-6.7.0/sip/Qt3DRender/qclearbuffers.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1630 2024-04-20 16:01:00.186353 PyQt6_3D-6.7.0/sip/Qt3DRender/qclipplane.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1812 2024-04-20 16:01:00.199377 PyQt6_3D-6.7.0/sip/Qt3DRender/qcolormask.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2076 2024-04-20 16:01:00.174821 PyQt6_3D-6.7.0/sip/Qt3DRender/qcomputecommand.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1624 2024-04-20 16:01:00.191119 PyQt6_3D-6.7.0/sip/Qt3DRender/qcullface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1541 2024-04-20 16:01:00.199110 PyQt6_3D-6.7.0/sip/Qt3DRender/qdepthrange.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1772 2024-04-20 16:01:00.197401 PyQt6_3D-6.7.0/sip/Qt3DRender/qdepthtest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1511 2024-04-20 16:01:00.190855 PyQt6_3D-6.7.0/sip/Qt3DRender/qdirectionallight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1660 2024-04-20 16:01:00.193225 PyQt6_3D-6.7.0/sip/Qt3DRender/qdispatchcompute.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1258 2024-04-20 16:01:00.190385 PyQt6_3D-6.7.0/sip/Qt3DRender/qdithering.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2073 2024-04-20 16:01:00.204445 PyQt6_3D-6.7.0/sip/Qt3DRender/qeffect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1777 2024-04-20 16:01:00.191380 PyQt6_3D-6.7.0/sip/Qt3DRender/qenvironmentlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1536 2024-04-20 16:01:00.182808 PyQt6_3D-6.7.0/sip/Qt3DRender/qfilterkey.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1346 2024-04-20 16:01:00.203861 PyQt6_3D-6.7.0/sip/Qt3DRender/qframegraphnode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1645 2024-04-20 16:01:00.202441 PyQt6_3D-6.7.0/sip/Qt3DRender/qfrontface.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1291 2024-04-20 16:01:00.196593 PyQt6_3D-6.7.0/sip/Qt3DRender/qfrustumculling.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3672 2024-04-20 16:01:00.190159 PyQt6_3D-6.7.0/sip/Qt3DRender/qgeometryrenderer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2605 2024-04-20 16:01:00.174470 PyQt6_3D-6.7.0/sip/Qt3DRender/qgraphicsapifilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1352 2024-04-20 16:01:00.179065 PyQt6_3D-6.7.0/sip/Qt3DRender/qlayer.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2119 2024-04-20 16:01:00.192965 PyQt6_3D-6.7.0/sip/Qt3DRender/qlayerfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2589 2024-04-20 16:01:00.180287 PyQt6_3D-6.7.0/sip/Qt3DRender/qlevelofdetail.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1682 2024-04-20 16:01:00.196150 PyQt6_3D-6.7.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1320 2024-04-20 16:01:00.198863 PyQt6_3D-6.7.0/sip/Qt3DRender/qlevelofdetailswitch.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1505 2024-04-20 16:01:00.177693 PyQt6_3D-6.7.0/sip/Qt3DRender/qlinewidth.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7581 2024-04-20 16:01:00.201412 PyQt6_3D-6.7.0/sip/Qt3DRender/qlist.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1642 2024-04-20 16:01:00.195205 PyQt6_3D-6.7.0/sip/Qt3DRender/qmaterial.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2107 2024-04-20 16:01:00.204161 PyQt6_3D-6.7.0/sip/Qt3DRender/qmemorybarrier.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1804 2024-04-20 16:01:00.183620 PyQt6_3D-6.7.0/sip/Qt3DRender/qmesh.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1342 2024-04-20 16:01:00.186912 PyQt6_3D-6.7.0/sip/Qt3DRender/qmultisampleantialiasing.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1270 2024-04-20 16:01:00.194069 PyQt6_3D-6.7.0/sip/Qt3DRender/qnodepthmask.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1243 2024-04-20 16:01:00.201928 PyQt6_3D-6.7.0/sip/Qt3DRender/qnodraw.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1261 2024-04-20 16:01:00.196366 PyQt6_3D-6.7.0/sip/Qt3DRender/qnopicking.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2112 2024-04-20 16:01:00.178837 PyQt6_3D-6.7.0/sip/Qt3DRender/qobjectpicker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1857 2024-04-20 16:01:00.178214 PyQt6_3D-6.7.0/sip/Qt3DRender/qpaintedtextureimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1759 2024-04-20 16:01:00.176127 PyQt6_3D-6.7.0/sip/Qt3DRender/qparameter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2421 2024-04-20 16:01:00.197748 PyQt6_3D-6.7.0/sip/Qt3DRender/qpickevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1277 2024-04-20 16:01:00.175069 PyQt6_3D-6.7.0/sip/Qt3DRender/qpickingproxy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2962 2024-04-20 16:01:00.174097 PyQt6_3D-6.7.0/sip/Qt3DRender/qpickingsettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1590 2024-04-20 16:01:00.181546 PyQt6_3D-6.7.0/sip/Qt3DRender/qpicklineevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1491 2024-04-20 16:01:00.182309 PyQt6_3D-6.7.0/sip/Qt3DRender/qpickpointevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1951 2024-04-20 16:01:00.196842 PyQt6_3D-6.7.0/sip/Qt3DRender/qpicktriangleevent.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1778 2024-04-20 16:01:00.198014 PyQt6_3D-6.7.0/sip/Qt3DRender/qpointlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1705 2024-04-20 16:01:00.184895 PyQt6_3D-6.7.0/sip/Qt3DRender/qpointsize.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1580 2024-04-20 16:01:00.185614 PyQt6_3D-6.7.0/sip/Qt3DRender/qpolygonoffset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1644 2024-04-20 16:01:00.187211 PyQt6_3D-6.7.0/sip/Qt3DRender/qproximityfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1931 2024-04-20 16:01:00.197129 PyQt6_3D-6.7.0/sip/Qt3DRender/qrastermode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1807 2024-04-20 16:01:00.195906 PyQt6_3D-6.7.0/sip/Qt3DRender/qraycaster.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2004 2024-04-20 16:01:00.175371 PyQt6_3D-6.7.0/sip/Qt3DRender/qraycasterhit.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1151 2024-04-20 16:01:00.187482 PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderapi.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1562 2024-04-20 16:01:00.176941 PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderaspect.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2747 2024-04-20 16:01:00.186022 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendercapabilities.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1860 2024-04-20 16:01:00.200294 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendercapture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2795 2024-04-20 16:01:00.192663 PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderpass.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2147 2024-04-20 16:01:00.180987 PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderpassfilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2043 2024-04-20 16:01:00.194359 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendersettings.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1203 2024-04-20 16:01:00.195415 PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderstate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1726 2024-04-20 16:01:00.202697 PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderstateset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1811 2024-04-20 16:01:00.182564 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendersurfaceselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1710 2024-04-20 16:01:00.202179 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendertarget.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2826 2024-04-20 16:01:00.198371 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendertargetoutput.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1552 2024-04-20 16:01:00.177929 PyQt6_3D-6.7.0/sip/Qt3DRender/qrendertargetselector.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2175 2024-04-20 16:01:00.187852 PyQt6_3D-6.7.0/sip/Qt3DRender/qsceneloader.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1704 2024-04-20 16:01:00.172533 PyQt6_3D-6.7.0/sip/Qt3DRender/qscissortest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1540 2024-04-20 16:01:00.183057 PyQt6_3D-6.7.0/sip/Qt3DRender/qscreenraycaster.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1294 2024-04-20 16:01:00.186641 PyQt6_3D-6.7.0/sip/Qt3DRender/qseamlesscubemap.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1582 2024-04-20 16:01:00.189144 PyQt6_3D-6.7.0/sip/Qt3DRender/qsetfence.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1697 2024-04-20 16:01:00.175644 PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderdata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3214 2024-04-20 16:01:00.173339 PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3725 2024-04-20 16:01:00.180695 PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderprogram.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3785 2024-04-20 16:01:00.172888 PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderprogrambuilder.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1911 2024-04-20 16:01:00.193512 PyQt6_3D-6.7.0/sip/Qt3DRender/qsortpolicy.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2083 2024-04-20 16:01:00.176687 PyQt6_3D-6.7.0/sip/Qt3DRender/qspotlight.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1602 2024-04-20 16:01:00.198632 PyQt6_3D-6.7.0/sip/Qt3DRender/qstencilmask.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1425 2024-04-20 16:01:00.177167 PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciloperation.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2785 2024-04-20 16:01:00.178552 PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciloperationarguments.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1385 2024-04-20 16:01:00.195639 PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciltest.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2416 2024-04-20 16:01:00.194681 PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciltestarguments.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1662 2024-04-20 16:01:00.177430 PyQt6_3D-6.7.0/sip/Qt3DRender/qsubtreeenabler.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2579 2024-04-20 16:01:00.193844 PyQt6_3D-6.7.0/sip/Qt3DRender/qtechnique.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2125 2024-04-20 16:01:00.184260 PyQt6_3D-6.7.0/sip/Qt3DRender/qtechniquefilter.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4735 2024-04-20 16:01:00.192043 PyQt6_3D-6.7.0/sip/Qt3DRender/qtexture.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3172 2024-04-20 16:01:00.183937 PyQt6_3D-6.7.0/sip/Qt3DRender/qtexturedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2108 2024-04-20 16:01:00.176399 PyQt6_3D-6.7.0/sip/Qt3DRender/qtexturedataupdate.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2048 2024-04-20 16:01:00.173687 PyQt6_3D-6.7.0/sip/Qt3DRender/qtextureimage.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2474 2024-04-20 16:01:00.189733 PyQt6_3D-6.7.0/sip/Qt3DRender/qtextureimagedata.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1546 2024-04-20 16:01:00.175876 PyQt6_3D-6.7.0/sip/Qt3DRender/qtextureimagedatagenerator.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2337 2024-04-20 16:01:00.184583 PyQt6_3D-6.7.0/sip/Qt3DRender/qtexturewrapmode.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1606 2024-04-20 16:01:00.194948 PyQt6_3D-6.7.0/sip/Qt3DRender/qviewport.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1950 2024-04-20 16:01:00.182077 PyQt6_3D-6.7.0/sip/Qt3DRender/qwaitfence.sip
```

### Comparing `PyQt6_3D-6.6.0/ChangeLog` & `PyQt6_3D-6.7.0/ChangeLog`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+2024-04-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Updated for Qt v6.7.0.
+	[78386dd50be5] [6.7.0]
+
+2024-03-17  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-3D.msp:
+	Added support for Qt v6.7.
+	[9d1e6aa64d73]
+
+2024-02-18  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Updated the NEWS file.
+	[becf0a1463f2]
+
+	* README, README.md, pyproject.toml:
+	Migrated from [tool.sip.metadata] to [project] in pyproject.toml.
+	[0af498f877ee]
+
+	* Merged the 6.6-maint branch.
+	[3609a305f878]
+
+2024-01-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, rb-product.toml:
+	Removed the product file.
+	[b57075719357] <6.6-maint>
+
+2023-10-25  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 6.6.0 for changeset b0379b68ceac
+	[90c4512e1f27]
+
 2023-10-22  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-3D.msp:
 	Updated for Qt v6.6.
 	[b0379b68ceac] [6.6.0]
 
 2023-04-04  Phil Thompson  <phil@riverbankcomputing.com>
```

### Comparing `PyQt6_3D-6.6.0/LICENSE` & `PyQt6_3D-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/NEWS` & `PyQt6_3D-6.7.0/NEWS`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+v6.7.0 4th April 2024
+  - Added support for Qt v6.7.
+
 v6.6.0 22nd October 2023
   - Added support for Qt v6.6.
 
 v6.5.0 31st March 2023
   - Added support for Qt v6.5.
 
 v6.4.0 30th September 2022
```

### Comparing `PyQt6_3D-6.6.0/PKG-INFO` & `PyQt6_3D-6.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 Metadata-Version: 2.1
 Name: PyQt6-3D
-Version: 6.6.0
-Requires-Python: >=3.7
+Version: 6.7.0
+Requires-Python: >=3.8
 Summary: Python bindings for the Qt 3D framework
-Home-Page: https://www.riverbankcomputing.com/software/pyqt3d/
-Author: Riverbank Computing Limited
-Author-Email: info@riverbankcomputing.com
-License: GPL v3
+Description-Content-Type: text/markdown
+Project-Url: homepage, https://www.riverbankcomputing.com/software/pyqt3d/
 Requires-Dist: PyQt6 (>=6.2.0)
+License: GPL v3
+Author-Email: Riverbank Computing Limited <info@riverbankcomputing.com>
 
-PyQt6-3D - Python Bindings for the Qt 3D Framework
-==================================================
+# PyQt6-3D - Python Bindings for the Qt 3D Framework
 
 PyQt6-3D is a set of Python bindings for The Qt Company's Qt 3D framework.  The
 bindings sit on top of PyQt6 and are implemented as six separate modules
 corresponding to the different libraries that make up the framework.
 
 
-Author
-------
+## Author
 
 PyQt6-3D is copyright (c) Riverbank Computing Limited.  Its homepage is
 https://www.riverbankcomputing.com/software/pyqt3d/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-3D is released under the GPL v3 license and under a commercial license
 that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-3D can be installed from PyPI::
+The GPL version of PyQt6-3D can be installed from PyPI:
 
     pip install PyQt6-3D
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_3D-6.6.0/README` & `PyQt6_3D-6.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-PyQt6-3D - Python Bindings for the Qt 3D Framework
-==================================================
+# PyQt6-3D - Python Bindings for the Qt 3D Framework
 
 PyQt6-3D is a set of Python bindings for The Qt Company's Qt 3D framework.  The
 bindings sit on top of PyQt6 and are implemented as six separate modules
 corresponding to the different libraries that make up the framework.
 
 
-Author
-------
+## Author
 
 PyQt6-3D is copyright (c) Riverbank Computing Limited.  Its homepage is
 https://www.riverbankcomputing.com/software/pyqt3d/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-3D is released under the GPL v3 license and under a commercial license
 that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-3D can be installed from PyPI::
+The GPL version of PyQt6-3D can be installed from PyPI:
 
     pip install PyQt6-3D
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_3D-6.6.0/examples/assets/chest/Chest.obj` & `PyQt6_3D-6.7.0/examples/assets/chest/Chest.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/chest/diffuse.webp` & `PyQt6_3D-6.7.0/examples/assets/chest/diffuse.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_negx.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_negx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_negy.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_negy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_negz.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_negz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_posx.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_posx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_posy.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_posy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/miramar/miramar_posz.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/miramar/miramar_posz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_negx.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_negx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_negy.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_negy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_negz.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_negz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_posx.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_posx.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_posy.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_posy.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/cubemaps/night/night_posz.webp` & `PyQt6_3D-6.7.0/examples/assets/cubemaps/night/night_posz.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/LICENSE.md` & `PyQt6_3D-6.7.0/examples/assets/gltf/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg` & `PyQt6_3D-6.7.0/examples/assets/gltf/wine/Wood_Cherry_Original_.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg` & `PyQt6_3D-6.7.0/examples/assets/gltf/wine/_2004_old_vine_zinfandel_btl_xlg.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/wine/artezin_bottle.jpg` & `PyQt6_3D-6.7.0/examples/assets/gltf/wine/artezin_bottle.jpg`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine.bin` & `PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine.bin`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine.dae` & `PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine.dae`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/gltf/wine/wine.gltf` & `PyQt6_3D-6.7.0/examples/assets/gltf/wine/wine.gltf`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/bamboo.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/bamboo.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/bamboo_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/bamboo_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cover.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cover.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cover_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cover_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-bamboo.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-palm.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-pine.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-pot-cover.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-pot.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-shrub.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cross-spikes.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cross-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-bamboo.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-palm.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-pine.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-pot-cover.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-pot.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-shrub.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/cylinder-spikes.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/cylinder-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/palm.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/palm.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/palm_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/palm_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/pine.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/pine.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/pine_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/pine_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/pot.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/pot.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/pot_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/pot_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/shrub.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/shrub.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/shrub_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/shrub_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-bamboo.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-palm.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-pine.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-pot-cover.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-pot.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-shrub.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/sphere-spikes.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/sphere-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/spikes.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/spikes.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/spikes_normal.webp` & `PyQt6_3D-6.7.0/examples/assets/houseplants/spikes_normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-bamboo.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-palm.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-pine.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-pot-cover.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-pot.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-shrub.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/square-spikes.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/square-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-bamboo.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-bamboo.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-palm.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-palm.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-pine.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-pine.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-pot-cover.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-pot-cover.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-pot.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-pot.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-shrub.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-shrub.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/houseplants/triangle-spikes.obj` & `PyQt6_3D-6.7.0/examples/assets/houseplants/triangle-spikes.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_black.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_black.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_blue.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_blue.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_green.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_green.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_red.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_red.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_rust.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_rust.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_stainless_steel.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_stainless_steel.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/diffus_yellow.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/diffus_yellow.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/metal_barrel.obj` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/metal_barrel.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_hard_bumps.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_hard_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_middle_bumps.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_middle_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_no_bumps.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_no_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/normal_soft_bumps.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/normal_soft_bumps.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/specular.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/specular.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/specular_rust.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/specular_rust.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/metalbarrel/specular_stainless_steel.webp` & `PyQt6_3D-6.7.0/examples/assets/metalbarrel/specular_stainless_steel.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/obj/ball.obj` & `PyQt6_3D-6.7.0/examples/assets/obj/ball.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/obj/toyplane.obj` & `PyQt6_3D-6.7.0/examples/assets/obj/toyplane.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/obj/trefoil.obj` & `PyQt6_3D-6.7.0/examples/assets/obj/trefoil.obj`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/test_scene.dae` & `PyQt6_3D-6.7.0/examples/assets/test_scene.dae`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/diffuse.webp` & `PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/diffuse.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/normal.webp` & `PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/normal.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/assets/textures/pattern_09/specular.webp` & `PyQt6_3D-6.7.0/examples/assets/textures/pattern_09/specular.webp`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/basicshapes-py.py` & `PyQt6_3D-6.7.0/examples/basicshapes-py.py`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/materials-py.py` & `PyQt6_3D-6.7.0/examples/materials-py.py`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/examples/simple-py.py` & `PyQt6_3D-6.7.0/examples/simple-py.py`

 * *Files identical despite different names*

### Comparing `PyQt6_3D-6.6.0/pyproject.toml` & `PyQt6_3D-6.7.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Specify the build system for the project.
 [build-system]
-requires = ["sip >=6, <7", "PyQt-builder >=1.9, <2"]
+requires = ["sip >=6.8, <7", "PyQt-builder >=1.9, <2"]
 build-backend = "sipbuild.api"
 
-# Specify the PEP 566 metadata for the project.
-[tool.sip.metadata]
+[project]
 name = "PyQt6-3D"
-version = "6.6.0"
-summary = "Python bindings for the Qt 3D framework"
-home-page = "https://www.riverbankcomputing.com/software/pyqt3d/"
-author = "Riverbank Computing Limited"
-author-email = "info@riverbankcomputing.com"
-license = "GPL v3"
-description-file = "README"
-requires-dist = "PyQt6 (>=6.2.0)"
+version = "6.7.0"
+description = "Python bindings for the Qt 3D framework"
+readme = "README.md"
+urls.homepage = "https://www.riverbankcomputing.com/software/pyqt3d/"
+dependencies = ["PyQt6 (>=6.2.0)"]
+license = {text = "GPL v3"}
+
+[[project.authors]]
+name = "Riverbank Computing Limited"
+email = "info@riverbankcomputing.com"
+
 
 # Specify a PyQt-based project.
 [tool.sip]
 project-factory = "pyqtbuild:PyQtProject"
 
 # Configure the project.
 [tool.sip.project]
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/Qt3DAnimationmod.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DAnimationmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -23,15 +23,15 @@
 %Module(name=PyQt6.Qt3DAnimation, keyword_arguments="Optional", use_limited_api=True)
 
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import Qt3DRender/Qt3DRendermod.sip
 %Import QtCore/QtCoremod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractanimation.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractanimation.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractanimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qabstractanimation.h>
 %End
 
-    class QAbstractAnimation : QObject /NoDefaultCtors/
+    class QAbstractAnimation : public QObject /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractanimation.h>
 %End
 
 %ConvertToSubClassCode
         static struct class_graph {
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractanimationclip.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractanimationclip.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractanimationclip.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qabstractanimationclip.h>
 %End
 
-    class QAbstractAnimationClip : Qt3DCore::QNode /NoDefaultCtors/
+    class QAbstractAnimationClip : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractanimationclip.h>
 %End
 
     public:
         virtual ~QAbstractAnimationClip();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractchannelmapping.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractchannelmapping.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractchannelmapping.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qabstractchannelmapping.h>
 %End
 
-    class QAbstractChannelMapping : Qt3DCore::QNode /NoDefaultCtors/
+    class QAbstractChannelMapping : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractchannelmapping.h>
 %End
 
     public:
         virtual ~QAbstractChannelMapping();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractclipanimator.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractclipanimator.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractclipanimator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qabstractclipanimator.h>
 %End
 
-    class QAbstractClipAnimator : Qt3DCore::QComponent
+    class QAbstractClipAnimator : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qabstractclipanimator.h>
 %End
 
     public:
         enum Loops
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qabstractclipblendnode.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qabstractclipblendnode.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractclipblendnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qabstractclipblendnode.h>
 %End
 
-    class QAbstractClipBlendNode : Qt3DCore::QNode
+    class QAbstractClipBlendNode : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qabstractclipblendnode.h>
 %End
 
     public:
         virtual ~QAbstractClipBlendNode();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qadditiveclipblend.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qadditiveclipblend.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qadditiveclipblend.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qadditiveclipblend.h>
 %End
 
-    class QAdditiveClipBlend : Qt3DAnimation::QAbstractClipBlendNode
+    class QAdditiveClipBlend : public Qt3DAnimation::QAbstractClipBlendNode
     {
 %TypeHeaderCode
 #include <qadditiveclipblend.h>
 %End
 
     public:
         explicit QAdditiveClipBlend(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationaspect.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationaspect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qanimationaspect.h>
 %End
 
-    class QAnimationAspect : Qt3DCore::QAbstractAspect
+    class QAnimationAspect : public Qt3DCore::QAbstractAspect
     {
 %TypeHeaderCode
 #include <qanimationaspect.h>
 %End
 
     public:
         explicit QAnimationAspect(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationclip.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationclip.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationclip.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qanimationclip.h>
 %End
 
-    class QAnimationClip : Qt3DAnimation::QAbstractAnimationClip
+    class QAnimationClip : public Qt3DAnimation::QAbstractAnimationClip
     {
 %TypeHeaderCode
 #include <qanimationclip.h>
 %End
 
     public:
         explicit QAnimationClip(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationclipdata.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationclipdata.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationclipdata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationcliploader.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationcliploader.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationcliploader.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qanimationcliploader.h>
 %End
 
-    class QAnimationClipLoader : Qt3DAnimation::QAbstractAnimationClip
+    class QAnimationClipLoader : public Qt3DAnimation::QAbstractAnimationClip
     {
 %TypeHeaderCode
 #include <qanimationcliploader.h>
 %End
 
     public:
         explicit QAnimationClipLoader(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationcontroller.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationcontroller.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationcontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qanimationcontroller.h>
 %End
 
-    class QAnimationController : QObject
+    class QAnimationController : public QObject
     {
 %TypeHeaderCode
 #include <qanimationcontroller.h>
 %End
 
     public:
         QAnimationController(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qanimationgroup.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qanimationgroup.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanimationgroup.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qanimationgroup.h>
 %End
 
-    class QAnimationGroup : QObject
+    class QAnimationGroup : public QObject
     {
 %TypeHeaderCode
 #include <qanimationgroup.h>
 %End
 
     public:
         explicit QAnimationGroup(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qblendedclipanimator.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qblendedclipanimator.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblendedclipanimator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qblendedclipanimator.h>
 %End
 
-    class QBlendedClipAnimator : Qt3DAnimation::QAbstractClipAnimator
+    class QBlendedClipAnimator : public Qt3DAnimation::QAbstractClipAnimator
     {
 %TypeHeaderCode
 #include <qblendedclipanimator.h>
 %End
 
     public:
         explicit QBlendedClipAnimator(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannel.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannel.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannel.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannelcomponent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannelcomponent.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannelcomponent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannelmapper.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannelmapper.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannelmapper.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qchannelmapper.h>
 %End
 
-    class QChannelMapper : Qt3DCore::QNode
+    class QChannelMapper : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qchannelmapper.h>
 %End
 
     public:
         explicit QChannelMapper(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qchannelmapping.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qchannelmapping.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchannelmapping.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qchannelmapping.h>
 %End
 
-    class QChannelMapping : Qt3DAnimation::QAbstractChannelMapping
+    class QChannelMapping : public Qt3DAnimation::QAbstractChannelMapping
     {
 %TypeHeaderCode
 #include <qchannelmapping.h>
 %End
 
     public:
         explicit QChannelMapping(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qclipanimator.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qclipanimator.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclipanimator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qclipanimator.h>
 %End
 
-    class QClipAnimator : Qt3DAnimation::QAbstractClipAnimator
+    class QClipAnimator : public Qt3DAnimation::QAbstractClipAnimator
     {
 %TypeHeaderCode
 #include <qclipanimator.h>
 %End
 
     public:
         explicit QClipAnimator(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qclipblendvalue.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qclipblendvalue.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclipblendvalue.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qclipblendvalue.h>
 %End
 
-    class QClipBlendValue : Qt3DAnimation::QAbstractClipBlendNode
+    class QClipBlendValue : public Qt3DAnimation::QAbstractClipBlendNode
     {
 %TypeHeaderCode
 #include <qclipblendvalue.h>
 %End
 
     public:
         explicit QClipBlendValue(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qclock.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qclock.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclock.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qclock.h>
 %End
 
-    class QClock : Qt3DCore::QNode
+    class QClock : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qclock.h>
 %End
 
     public:
         explicit QClock(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qkeyframe.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qkeyframe.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyframe.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qkeyframeanimation.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qkeyframeanimation.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyframeanimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qkeyframeanimation.h>
 %End
 
-    class QKeyframeAnimation : Qt3DAnimation::QAbstractAnimation
+    class QKeyframeAnimation : public Qt3DAnimation::QAbstractAnimation
     {
 %TypeHeaderCode
 #include <qkeyframeanimation.h>
 %End
 
     public:
         explicit QKeyframeAnimation(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qlerpclipblend.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qlerpclipblend.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlerpclipblend.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qlerpclipblend.h>
 %End
 
-    class QLerpClipBlend : Qt3DAnimation::QAbstractClipBlendNode
+    class QLerpClipBlend : public Qt3DAnimation::QAbstractClipBlendNode
     {
 %TypeHeaderCode
 #include <qlerpclipblend.h>
 %End
 
     public:
         explicit QLerpClipBlend(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qmorphinganimation.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qmorphinganimation.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmorphinganimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qmorphinganimation.h>
 %End
 
-    class QMorphingAnimation : Qt3DAnimation::QAbstractAnimation
+    class QMorphingAnimation : public Qt3DAnimation::QAbstractAnimation
     {
 %TypeHeaderCode
 #include <qmorphinganimation.h>
 %End
 
     public:
         enum Method
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qmorphtarget.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qmorphtarget.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmorphtarget.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qmorphtarget.h>
 %End
 
-    class QMorphTarget : QObject
+    class QMorphTarget : public QObject
     {
 %TypeHeaderCode
 #include <qmorphtarget.h>
 %End
 
     public:
         explicit QMorphTarget(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qskeletonmapping.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qskeletonmapping.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskeletonmapping.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qskeletonmapping.h>
 %End
 
-    class QSkeletonMapping : Qt3DAnimation::QAbstractChannelMapping
+    class QSkeletonMapping : public Qt3DAnimation::QAbstractChannelMapping
     {
 %TypeHeaderCode
 #include <qskeletonmapping.h>
 %End
 
     public:
         explicit QSkeletonMapping(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DAnimation/qvertexblendanimation.sip` & `PyQt6_3D-6.7.0/sip/Qt3DAnimation/qvertexblendanimation.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvertexblendanimation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DAnimation Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DAnimation
 {
 %TypeHeaderCode
 #include <qvertexblendanimation.h>
 %End
 
-    class QVertexBlendAnimation : Qt3DAnimation::QAbstractAnimation
+    class QVertexBlendAnimation : public Qt3DAnimation::QAbstractAnimation
     {
 %TypeHeaderCode
 #include <qvertexblendanimation.h>
 %End
 
     public:
         explicit QVertexBlendAnimation(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/Qt3DCoremod.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/Qt3DCoremod.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DCoremod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,18 +21,18 @@
 
 
 %Module(name=PyQt6.Qt3DCore, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 
-%Timeline {Qt3D_6_0_0 Qt3D_6_1_0 Qt3D_6_2_0 Qt3D_6_3_0 Qt3D_6_4_0 Qt3D_6_5_0 Qt3D_6_6_0}
+%Timeline {Qt3D_6_0_0 Qt3D_6_1_0 Qt3D_6_2_0 Qt3D_6_3_0 Qt3D_6_4_0 Qt3D_6_5_0 Qt3D_6_6_0 Qt3D_6_7_0}
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -49,16 +49,16 @@
 %DefaultSupertype PyQt6.sip.simplewrapper
 %HideNamespace Qt3DCore
 
 int PYQT_3D_VERSION;
 const char *PYQT_3D_VERSION_STR;
 
 %ModuleCode
-static int PYQT_3D_VERSION = 0x060600;
-static const char *PYQT_3D_VERSION_STR = "6.6.0";
+static int PYQT_3D_VERSION = 0x060700;
+static const char *PYQT_3D_VERSION_STR = "6.7.0";
 %End
 
 %Include qabstractaspect.sip
 %Include qabstractfunctor.sip
 %Include qabstractskeleton.sip
 %Include qarmature.sip
 %Include qaspectengine.sip
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qabstractaspect.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qabstractaspect.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 {
 %TypeHeaderCode
 #include <qabstractaspect.h>
 %End
 
     typedef QSharedPointer<Qt3DCore::QBackendNodeMapper> QBackendNodeMapperPtr;
 
-    class QAbstractAspect : QObject
+    class QAbstractAspect : public QObject
     {
 %TypeHeaderCode
 #include <qabstractaspect.h>
 %End
 
     public:
         explicit QAbstractAspect(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qabstractfunctor.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qabstractfunctor.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractfunctor.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qabstractskeleton.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qabstractskeleton.sip`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractskeleton.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qabstractskeleton.h>
 %End
 
-    class QAbstractSkeleton : Qt3DCore::QNode /NoDefaultCtors/
+    class QAbstractSkeleton : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractskeleton.h>
 %End
 
     public:
         virtual ~QAbstractSkeleton();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qarmature.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qarmature.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qarmature.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qarmature.h>
 %End
 
-    class QArmature : Qt3DCore::QComponent
+    class QArmature : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qarmature.h>
 %End
 
     public:
         explicit QArmature(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qaspectengine.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qaspectengine.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaspectengine.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 {
 %TypeHeaderCode
 #include <qaspectengine.h>
 %End
 
     typedef QSharedPointer<Qt3DCore::QEntity> QEntityPtr;
 
-    class QAspectEngine : QObject
+    class QAspectEngine : public QObject
     {
 %TypeHeaderCode
 #include <qaspectengine.h>
 %End
 
     public:
         explicit QAspectEngine(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qattribute.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qattribute.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qattribute.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 {
 %TypeHeaderCode
 #include <qattribute.h>
 %End
 
     typedef QSharedPointer<Qt3DCore::QBuffer> QBufferPtr;
 
-    class QAttribute : Qt3DCore::QNode
+    class QAttribute : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qattribute.h>
 %End
 
     public:
         enum AttributeType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qbackendnode.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qbackendnode.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbackendnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qboundingvolume.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qboundingvolume.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboundingvolume.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qboundingvolume.h>
 %End
 
-    class QBoundingVolume : Qt3DCore::QComponent
+    class QBoundingVolume : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qboundingvolume.h>
 %End
 
     public:
         explicit QBoundingVolume(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qbuffer.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qbuffer.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbuffer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qbuffer.h>
 %End
 
-    class QBuffer : Qt3DCore::QNode
+    class QBuffer : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qbuffer.h>
 %End
 
     public:
         enum UsageType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qcomponent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qcomponent.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcomponent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qcomponent.h>
 %End
 
-    class QComponent : Qt3DCore::QNode
+    class QComponent : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qcomponent.h>
 %End
 
     public:
         explicit QComponent(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qcoresettings.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qcoresettings.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcoresettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qcoresettings.h>
 %End
 
-    class QCoreSettings : Qt3DCore::QComponent
+    class QCoreSettings : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qcoresettings.h>
 %End
 
     public:
         explicit QCoreSettings(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qentity.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qentity.sip`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qentity.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 {
 %TypeHeaderCode
 #include <qentity.h>
 %End
 
     typedef QList<Qt3DCore::QComponent *> QComponentVector;
 
-    class QEntity : Qt3DCore::QNode
+    class QEntity : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qentity.h>
 %End
 
     public:
         explicit QEntity(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qgeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qgeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qgeometry.h>
 %End
 
-    class QGeometry : Qt3DCore::QNode
+    class QGeometry : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qgeometry.h>
 %End
 
     public:
         explicit QGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qgeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qgeometryview.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qgeometryview.h>
 %End
 
-    class QGeometryView : Qt3DCore::QNode
+    class QGeometryView : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qgeometryview.h>
 %End
 
     public:
         enum PrimitiveType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qjoint.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qjoint.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qjoint.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qjoint.h>
 %End
 
-    class QJoint : Qt3DCore::QNode
+    class QJoint : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qjoint.h>
 %End
 
     public:
         explicit QJoint(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qnode.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qnode.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 {
 %TypeHeaderCode
 #include <qnode.h>
 %End
 
     typedef QList<Qt3DCore::QNode *> QNodeVector;
 
-    class QNode : QObject
+    class QNode : public QObject
     {
 %TypeHeaderCode
 #include <qnode.h>
 %End
 
 %ConvertToSubClassCode
         static struct class_graph {
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qnodeid.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qnodeid.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnodeid.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qsharedpointer.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qsharedpointer.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // This is the SIP interface definition for the QSharedPointer based mapped
 // types specific to PyQt3D.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qskeleton.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qskeleton.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskeleton.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qskeleton.h>
 %End
 
-    class QSkeleton : Qt3DCore::QAbstractSkeleton
+    class QSkeleton : public Qt3DCore::QAbstractSkeleton
     {
 %TypeHeaderCode
 #include <qskeleton.h>
 %End
 
     public:
         QSkeleton(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qskeletonloader.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qskeletonloader.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskeletonloader.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qskeletonloader.h>
 %End
 
-    class QSkeletonLoader : Qt3DCore::QAbstractSkeleton
+    class QSkeletonLoader : public Qt3DCore::QAbstractSkeleton
     {
 %TypeHeaderCode
 #include <qskeletonloader.h>
 %End
 
     public:
         explicit QSkeletonLoader(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DCore/qtransform.sip` & `PyQt6_3D-6.7.0/sip/Qt3DCore/qtransform.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtransform.sip generated by MetaSIP
 //
 // This file is part of the Qt3DCore Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DCore
 {
 %TypeHeaderCode
 #include <qtransform.h>
 %End
 
-    class QTransform : Qt3DCore::QComponent
+    class QTransform : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qtransform.h>
 %End
 
     public:
         explicit QTransform(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/Qt3DExtrasmod.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/Qt3DExtrasmod.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DExtrasmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -25,15 +25,15 @@
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import Qt3DInput/Qt3DInputmod.sip
 %Import Qt3DRender/Qt3DRendermod.sip
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qabstractcameracontroller.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qabstractcameracontroller.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractcameracontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qabstractcameracontroller.h>
 %End
 
-    class QAbstractCameraController : Qt3DCore::QEntity /Abstract/
+    class QAbstractCameraController : public Qt3DCore::QEntity /Abstract/
     {
 %TypeHeaderCode
 #include <qabstractcameracontroller.h>
 %End
 
     public:
         virtual ~QAbstractCameraController();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qabstractspritesheet.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qabstractspritesheet.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractspritesheet.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qabstractspritesheet.h>
 %End
 
-    class QAbstractSpriteSheet : Qt3DCore::QNode /NoDefaultCtors/
+    class QAbstractSpriteSheet : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractspritesheet.h>
 %End
 
     public:
         virtual ~QAbstractSpriteSheet();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qconegeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qconegeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qconegeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qconegeometry.h>
 %End
 
-    class QConeGeometry : Qt3DCore::QGeometry
+    class QConeGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qconegeometry.h>
 %End
 
     public:
         explicit QConeGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qconegeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qconegeometryview.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qconegeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qconegeometryview.h>
 %End
 
-    class QConeGeometryView : Qt3DCore::QGeometryView
+    class QConeGeometryView : public Qt3DCore::QGeometryView
     {
 %TypeHeaderCode
 #include <qconegeometryview.h>
 %End
 
     public:
         explicit QConeGeometryView(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qconemesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qconemesh.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qconemesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qconemesh.h>
 %End
 
-    class QConeMesh : Qt3DRender::QGeometryRenderer
+    class QConeMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qconemesh.h>
 %End
 
     public:
         explicit QConeMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qcuboidgeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qcuboidgeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcuboidgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qcuboidgeometry.h>
 %End
 
-    class QCuboidGeometry : Qt3DCore::QGeometry
+    class QCuboidGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qcuboidgeometry.h>
 %End
 
     public:
         explicit QCuboidGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qcuboidgeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qcuboidgeometryview.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcuboidgeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qcuboidgeometryview.h>
 %End
 
-    class QCuboidGeometryView : Qt3DCore::QGeometryView
+    class QCuboidGeometryView : public Qt3DCore::QGeometryView
     {
 %TypeHeaderCode
 #include <qcuboidgeometryview.h>
 %End
 
     public:
         explicit QCuboidGeometryView(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qcuboidmesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qcuboidmesh.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcuboidmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qcuboidmesh.h>
 %End
 
-    class QCuboidMesh : Qt3DRender::QGeometryRenderer
+    class QCuboidMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qcuboidmesh.h>
 %End
 
     public:
         explicit QCuboidMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qcylindergeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qcylindergeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcylindergeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qcylindergeometry.h>
 %End
 
-    class QCylinderGeometry : Qt3DCore::QGeometry
+    class QCylinderGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qcylindergeometry.h>
 %End
 
     public:
         explicit QCylinderGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qcylindergeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qcylindergeometryview.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcylindergeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qcylindergeometryview.h>
 %End
 
-    class QCylinderGeometryView : Qt3DCore::QGeometryView
+    class QCylinderGeometryView : public Qt3DCore::QGeometryView
     {
 %TypeHeaderCode
 #include <qcylindergeometryview.h>
 %End
 
     public:
         explicit QCylinderGeometryView(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qcylindermesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qcylindermesh.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcylindermesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qcylindermesh.h>
 %End
 
-    class QCylinderMesh : Qt3DRender::QGeometryRenderer
+    class QCylinderMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qcylindermesh.h>
 %End
 
     public:
         explicit QCylinderMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qdiffusemapmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qdiffusemapmaterial.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdiffusemapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qdiffusemapmaterial.h>
 %End
 
-    class QDiffuseMapMaterial : Qt3DRender::QMaterial
+    class QDiffuseMapMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qdiffusemapmaterial.h>
 %End
 
     public:
         explicit QDiffuseMapMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qdiffusespecularmapmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdiffusespecularmapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qdiffusespecularmapmaterial.h>
 %End
 
-    class QDiffuseSpecularMapMaterial : Qt3DRender::QMaterial
+    class QDiffuseSpecularMapMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qdiffusespecularmapmaterial.h>
 %End
 
     public:
         explicit QDiffuseSpecularMapMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qdiffusespecularmaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdiffusespecularmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qdiffusespecularmaterial.h>
 %End
 
-    class QDiffuseSpecularMaterial : Qt3DRender::QMaterial
+    class QDiffuseSpecularMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qdiffusespecularmaterial.h>
 %End
 
     public:
         explicit QDiffuseSpecularMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qextrudedtextgeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qextrudedtextgeometry.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qextrudedtextgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qextrudedtextgeometry.h>
 %End
 
-    class QExtrudedTextGeometry : Qt3DCore::QGeometry
+    class QExtrudedTextGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qextrudedtextgeometry.h>
 %End
 
     public:
         explicit QExtrudedTextGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qextrudedtextmesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qextrudedtextmesh.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qextrudedtextmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qextrudedtextmesh.h>
 %End
 
-    class QExtrudedTextMesh : Qt3DRender::QGeometryRenderer
+    class QExtrudedTextMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qextrudedtextmesh.h>
 %End
 
     public:
         explicit QExtrudedTextMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qfirstpersoncameracontroller.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfirstpersoncameracontroller.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qfirstpersoncameracontroller.h>
 %End
 
-    class QFirstPersonCameraController : Qt3DExtras::QAbstractCameraController
+    class QFirstPersonCameraController : public Qt3DExtras::QAbstractCameraController
     {
 %TypeHeaderCode
 #include <qfirstpersoncameracontroller.h>
 %End
 
     public:
         explicit QFirstPersonCameraController(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qforwardrenderer.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qforwardrenderer.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qforwardrenderer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qforwardrenderer.h>
 %End
 
-    class QForwardRenderer : Qt3DRender::QTechniqueFilter
+    class QForwardRenderer : public Qt3DRender::QTechniqueFilter
     {
 %TypeHeaderCode
 #include <qforwardrenderer.h>
 %End
 
     public:
         explicit QForwardRenderer(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qgoochmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qgoochmaterial.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgoochmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qgoochmaterial.h>
 %End
 
-    class QGoochMaterial : Qt3DRender::QMaterial
+    class QGoochMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qgoochmaterial.h>
 %End
 
     public:
         explicit QGoochMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qmetalroughmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qmetalroughmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmetalroughmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qmetalroughmaterial.h>
 %End
 
-    class QMetalRoughMaterial : Qt3DRender::QMaterial
+    class QMetalRoughMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qmetalroughmaterial.h>
 %End
 
     public:
         explicit QMetalRoughMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qmorphphongmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qmorphphongmaterial.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmorphphongmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qmorphphongmaterial.h>
 %End
 
-    class QMorphPhongMaterial : Qt3DRender::QMaterial
+    class QMorphPhongMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qmorphphongmaterial.h>
 %End
 
     public:
         explicit QMorphPhongMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qnormaldiffusemapalphamaterial.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnormaldiffusemapalphamaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qnormaldiffusemapalphamaterial.h>
 %End
 
-    class QNormalDiffuseMapAlphaMaterial : Qt3DExtras::QNormalDiffuseMapMaterial
+    class QNormalDiffuseMapAlphaMaterial : public Qt3DExtras::QNormalDiffuseMapMaterial
     {
 %TypeHeaderCode
 #include <qnormaldiffusemapalphamaterial.h>
 %End
 
     public:
         explicit QNormalDiffuseMapAlphaMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qnormaldiffusemapmaterial.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnormaldiffusemapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qnormaldiffusemapmaterial.h>
 %End
 
-    class QNormalDiffuseMapMaterial : Qt3DRender::QMaterial
+    class QNormalDiffuseMapMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qnormaldiffusemapmaterial.h>
 %End
 
     public:
         explicit QNormalDiffuseMapMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qnormaldiffusespecularmapmaterial.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnormaldiffusespecularmapmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qnormaldiffusespecularmapmaterial.h>
 %End
 
-    class QNormalDiffuseSpecularMapMaterial : Qt3DRender::QMaterial
+    class QNormalDiffuseSpecularMapMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qnormaldiffusespecularmapmaterial.h>
 %End
 
     public:
         explicit QNormalDiffuseSpecularMapMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qorbitcameracontroller.sip` & `PyQt6_3D-6.7.0/sip/Qt3DLogic/qlogicaspect.sip`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qorbitcameracontroller.sip generated by MetaSIP
+// qlogicaspect.sip generated by MetaSIP
 //
-// This file is part of the Qt3DExtras Python extension module.
+// This file is part of the Qt3DLogic Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,29 +16,24 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-namespace Qt3DExtras
+namespace Qt3DLogic
 {
 %TypeHeaderCode
-#include <qorbitcameracontroller.h>
+#include <qlogicaspect.h>
 %End
 
-    class QOrbitCameraController : Qt3DExtras::QAbstractCameraController
+    class QLogicAspect : public Qt3DCore::QAbstractAspect
     {
 %TypeHeaderCode
-#include <qorbitcameracontroller.h>
+#include <qlogicaspect.h>
 %End
 
     public:
-        explicit QOrbitCameraController(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QOrbitCameraController();
-        float zoomInLimit() const;
-        void setZoomInLimit(float zoomInLimit);
-
-    signals:
-        void zoomInLimitChanged();
+        explicit QLogicAspect(QObject *parent /TransferThis/ = 0);
+        virtual ~QLogicAspect();
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qpervertexcolormaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qpervertexcolormaterial.sip`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpervertexcolormaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qpervertexcolormaterial.h>
 %End
 
-    class QPerVertexColorMaterial : Qt3DRender::QMaterial
+    class QPerVertexColorMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qpervertexcolormaterial.h>
 %End
 
     public:
         explicit QPerVertexColorMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qphongalphamaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qphongalphamaterial.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qphongalphamaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qphongalphamaterial.h>
 %End
 
-    class QPhongAlphaMaterial : Qt3DRender::QMaterial
+    class QPhongAlphaMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qphongalphamaterial.h>
 %End
 
     public:
         explicit QPhongAlphaMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qphongmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qphongmaterial.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qphongmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qphongmaterial.h>
 %End
 
-    class QPhongMaterial : Qt3DRender::QMaterial
+    class QPhongMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qphongmaterial.h>
 %End
 
     public:
         explicit QPhongMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qplanegeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qplanegeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qplanegeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qplanegeometry.h>
 %End
 
-    class QPlaneGeometry : Qt3DCore::QGeometry
+    class QPlaneGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qplanegeometry.h>
 %End
 
     public:
         explicit QPlaneGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qplanegeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qplanegeometryview.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qplanegeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qplanegeometryview.h>
 %End
 
-    class QPlaneGeometryView : Qt3DCore::QGeometryView
+    class QPlaneGeometryView : public Qt3DCore::QGeometryView
     {
 %TypeHeaderCode
 #include <qplanegeometryview.h>
 %End
 
     public:
         explicit QPlaneGeometryView(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qplanemesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qplanemesh.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qplanemesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qplanemesh.h>
 %End
 
-    class QPlaneMesh : Qt3DRender::QGeometryRenderer
+    class QPlaneMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qplanemesh.h>
 %End
 
     public:
         explicit QPlaneMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qskyboxentity.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qskyboxentity.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qskyboxentity.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qskyboxentity.h>
 %End
 
-    class QSkyboxEntity : Qt3DCore::QEntity
+    class QSkyboxEntity : public Qt3DCore::QEntity
     {
 %TypeHeaderCode
 #include <qskyboxentity.h>
 %End
 
     public:
         explicit QSkyboxEntity(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qspheregeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qspheregeometry.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspheregeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qspheregeometry.h>
 %End
 
-    class QSphereGeometry : Qt3DCore::QGeometry
+    class QSphereGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qspheregeometry.h>
 %End
 
     public:
         explicit QSphereGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qspheregeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qspheregeometryview.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspheregeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qspheregeometryview.h>
 %End
 
-    class QSphereGeometryView : Qt3DCore::QGeometryView
+    class QSphereGeometryView : public Qt3DCore::QGeometryView
     {
 %TypeHeaderCode
 #include <qspheregeometryview.h>
 %End
 
     public:
         explicit QSphereGeometryView(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qspheremesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qspheremesh.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspheremesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qspheremesh.h>
 %End
 
-    class QSphereMesh : Qt3DRender::QGeometryRenderer
+    class QSphereMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qspheremesh.h>
 %End
 
     public:
         explicit QSphereMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qspritegrid.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qspritegrid.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspritegrid.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qspritegrid.h>
 %End
 
-    class QSpriteGrid : Qt3DExtras::QAbstractSpriteSheet
+    class QSpriteGrid : public Qt3DExtras::QAbstractSpriteSheet
     {
 %TypeHeaderCode
 #include <qspritegrid.h>
 %End
 
     public:
         explicit QSpriteGrid(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qspritesheet.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qspritesheet.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspritesheet.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qspritesheet.h>
 %End
 
-    class QSpriteSheet : Qt3DExtras::QAbstractSpriteSheet
+    class QSpriteSheet : public Qt3DExtras::QAbstractSpriteSheet
     {
 %TypeHeaderCode
 #include <qspritesheet.h>
 %End
 
     public:
         explicit QSpriteSheet(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qspritesheetitem.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qspritesheetitem.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspritesheetitem.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qspritesheetitem.h>
 %End
 
-    class QSpriteSheetItem : Qt3DCore::QNode
+    class QSpriteSheetItem : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qspritesheetitem.h>
 %End
 
     public:
         explicit QSpriteSheetItem(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qt3dwindow.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qt3dwindow.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qt3dwindow.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qt3dwindow.h>
 %End
 
-    class Qt3DWindow : QWindow
+    class Qt3DWindow : public QWindow
     {
 %TypeHeaderCode
 #include <qt3dwindow.h>
 %End
 
 %ConvertToSubClassCode
         static struct class_graph {
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qtext2dentity.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qtext2dentity.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtext2dentity.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qtext2dentity.h>
 %End
 
-    class QText2DEntity : Qt3DCore::QEntity
+    class QText2DEntity : public Qt3DCore::QEntity
     {
 %TypeHeaderCode
 #include <qtext2dentity.h>
 %End
 
     public:
         explicit QText2DEntity(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qtexturematerial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qtexturematerial.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturematerial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qtexturematerial.h>
 %End
 
-    class QTextureMaterial : Qt3DRender::QMaterial
+    class QTextureMaterial : public Qt3DRender::QMaterial
     {
 %TypeHeaderCode
 #include <qtexturematerial.h>
 %End
 
     public:
         explicit QTextureMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qtorusgeometry.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qtorusgeometry.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtorusgeometry.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qtorusgeometry.h>
 %End
 
-    class QTorusGeometry : Qt3DCore::QGeometry
+    class QTorusGeometry : public Qt3DCore::QGeometry
     {
 %TypeHeaderCode
 #include <qtorusgeometry.h>
 %End
 
     public:
         explicit QTorusGeometry(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qtorusgeometryview.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qtorusgeometryview.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtorusgeometryview.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qtorusgeometryview.h>
 %End
 
-    class QTorusGeometryView : Qt3DCore::QGeometryView
+    class QTorusGeometryView : public Qt3DCore::QGeometryView
     {
 %TypeHeaderCode
 #include <qtorusgeometryview.h>
 %End
 
     public:
         explicit QTorusGeometryView(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DExtras/qtorusmesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DExtras/qtorusmesh.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtorusmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DExtras Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DExtras
 {
 %TypeHeaderCode
 #include <qtorusmesh.h>
 %End
 
-    class QTorusMesh : Qt3DRender::QGeometryRenderer
+    class QTorusMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qtorusmesh.h>
 %End
 
     public:
         explicit QTorusMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/Qt3DInputmod.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/Qt3DInputmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DInputmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -23,15 +23,15 @@
 %Module(name=PyQt6.Qt3DInput, keyword_arguments="Optional", use_limited_api=True)
 
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qabstractactioninput.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qabstractactioninput.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractactioninput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qabstractactioninput.h>
 %End
 
-    class QAbstractActionInput : Qt3DCore::QNode /NoDefaultCtors/
+    class QAbstractActionInput : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractactioninput.h>
 %End
 
     public:
         virtual ~QAbstractActionInput();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qabstractaxisinput.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qabstractaxisinput.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractaxisinput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qabstractaxisinput.h>
 %End
 
-    class QAbstractAxisInput : Qt3DCore::QNode /NoDefaultCtors/
+    class QAbstractAxisInput : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractaxisinput.h>
 %End
 
     public:
         virtual ~QAbstractAxisInput();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qabstractphysicaldevice.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qabstractphysicaldevice.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractphysicaldevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qabstractphysicaldevice.h>
 %End
 
-    class QAbstractPhysicalDevice : Qt3DCore::QNode
+    class QAbstractPhysicalDevice : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qabstractphysicaldevice.h>
 %End
 
 %ConvertToSubClassCode
         static struct class_graph {
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qaction.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qaction.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaction.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qaction.h>
 %End
 
-    class QAction : Qt3DCore::QNode
+    class QAction : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qaction.h>
 %End
 
     public:
         explicit QAction(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qactioninput.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qactioninput.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qactioninput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qactioninput.h>
 %End
 
-    class QActionInput : Qt3DInput::QAbstractActionInput
+    class QActionInput : public Qt3DInput::QAbstractActionInput
     {
 %TypeHeaderCode
 #include <qactioninput.h>
 %End
 
     public:
         explicit QActionInput(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qanalogaxisinput.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qanalogaxisinput.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qanalogaxisinput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qanalogaxisinput.h>
 %End
 
-    class QAnalogAxisInput : Qt3DInput::QAbstractAxisInput
+    class QAnalogAxisInput : public Qt3DInput::QAbstractAxisInput
     {
 %TypeHeaderCode
 #include <qanalogaxisinput.h>
 %End
 
     public:
         explicit QAnalogAxisInput(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qaxis.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qaxis.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaxis.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qaxis.h>
 %End
 
-    class QAxis : Qt3DCore::QNode
+    class QAxis : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qaxis.h>
 %End
 
     public:
         explicit QAxis(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qaxisaccumulator.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qaxisaccumulator.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaxisaccumulator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qaxisaccumulator.h>
 %End
 
-    class QAxisAccumulator : Qt3DCore::QComponent
+    class QAxisAccumulator : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qaxisaccumulator.h>
 %End
 
     public:
         enum SourceAxisType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qaxissetting.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qaxissetting.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qaxissetting.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qaxissetting.h>
 %End
 
-    class QAxisSetting : Qt3DCore::QNode
+    class QAxisSetting : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qaxissetting.h>
 %End
 
     public:
         explicit QAxisSetting(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qbuttonaxisinput.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qbuttonaxisinput.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbuttonaxisinput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qbuttonaxisinput.h>
 %End
 
-    class QButtonAxisInput : Qt3DInput::QAbstractAxisInput
+    class QButtonAxisInput : public Qt3DInput::QAbstractAxisInput
     {
 %TypeHeaderCode
 #include <qbuttonaxisinput.h>
 %End
 
     public:
         explicit QButtonAxisInput(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qinputaspect.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qinputaspect.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qinputaspect.h>
 %End
 
-    class QInputAspect : Qt3DCore::QAbstractAspect
+    class QInputAspect : public Qt3DCore::QAbstractAspect
     {
 %TypeHeaderCode
 #include <qinputaspect.h>
 %End
 
     public:
         explicit QInputAspect(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qinputchord.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qinputchord.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputchord.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qinputchord.h>
 %End
 
-    class QInputChord : Qt3DInput::QAbstractActionInput
+    class QInputChord : public Qt3DInput::QAbstractActionInput
     {
 %TypeHeaderCode
 #include <qinputchord.h>
 %End
 
     public:
         explicit QInputChord(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qinputsequence.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qinputsequence.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputsequence.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qinputsequence.h>
 %End
 
-    class QInputSequence : Qt3DInput::QAbstractActionInput
+    class QInputSequence : public Qt3DInput::QAbstractActionInput
     {
 %TypeHeaderCode
 #include <qinputsequence.h>
 %End
 
     public:
         explicit QInputSequence(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qinputsettings.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qinputsettings.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qinputsettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qinputsettings.h>
 %End
 
-    class QInputSettings : Qt3DCore::QComponent
+    class QInputSettings : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qinputsettings.h>
 %End
 
     public:
         explicit QInputSettings(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qkeyboarddevice.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qkeyboarddevice.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyboarddevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qkeyboarddevice.h>
 %End
 
-    class QKeyboardDevice : Qt3DInput::QAbstractPhysicalDevice
+    class QKeyboardDevice : public Qt3DInput::QAbstractPhysicalDevice
     {
 %TypeHeaderCode
 #include <qkeyboarddevice.h>
 %End
 
     public:
         explicit QKeyboardDevice(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qkeyboardhandler.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qkeyboardhandler.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyboardhandler.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qkeyboardhandler.h>
 %End
 
-    class QKeyboardHandler : Qt3DCore::QComponent
+    class QKeyboardHandler : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qkeyboardhandler.h>
 %End
 
     public:
         explicit QKeyboardHandler(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qkeyevent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qkeyevent.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qkeyevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qkeyevent.h>
 %End
 
-    class QKeyEvent : QObject
+    class QKeyEvent : public QObject
     {
 %TypeHeaderCode
 #include <qkeyevent.h>
 %End
 
     public:
         QKeyEvent(QEvent::Type type, int key, Qt::KeyboardModifiers modifiers, const QString &text = QString(), bool autorep = false, ushort count = 1);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qlogicaldevice.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qlogicaldevice.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogicaldevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qlogicaldevice.h>
 %End
 
-    class QLogicalDevice : Qt3DCore::QComponent
+    class QLogicalDevice : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qlogicaldevice.h>
 %End
 
     public:
         explicit QLogicalDevice(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qmousedevice.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qmousedevice.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmousedevice.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qmousedevice.h>
 %End
 
-    class QMouseDevice : Qt3DInput::QAbstractPhysicalDevice
+    class QMouseDevice : public Qt3DInput::QAbstractPhysicalDevice
     {
 %TypeHeaderCode
 #include <qmousedevice.h>
 %End
 
     public:
         explicit QMouseDevice(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qmouseevent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qmouseevent.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmouseevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qmouseevent.h>
 %End
 
-    class QMouseEvent : QObject
+    class QMouseEvent : public QObject
     {
 %TypeHeaderCode
 #include <qmouseevent.h>
 %End
 
     public:
         enum Buttons
@@ -61,15 +61,15 @@
         int buttons() const;
         Qt3DInput::QMouseEvent::Modifiers modifiers() const;
         bool isAccepted() const;
         void setAccepted(bool accepted);
         QEvent::Type type() const;
     };
 
-    class QWheelEvent : QObject
+    class QWheelEvent : public QObject
     {
 %TypeHeaderCode
 #include <qmouseevent.h>
 %End
 
     public:
         enum Buttons
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DInput/qmousehandler.sip` & `PyQt6_3D-6.7.0/sip/Qt3DInput/qmousehandler.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmousehandler.sip generated by MetaSIP
 //
 // This file is part of the Qt3DInput Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DInput
 {
 %TypeHeaderCode
 #include <qmousehandler.h>
 %End
 
-    class QMouseHandler : Qt3DCore::QComponent
+    class QMouseHandler : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qmousehandler.h>
 %End
 
     public:
         explicit QMouseHandler(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DLogic/Qt3DLogicmod.sip` & `PyQt6_3D-6.7.0/sip/Qt3DLogic/Qt3DLogicmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DLogicmod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DLogic Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,15 +21,15 @@
 
 
 %Module(name=PyQt6.Qt3DLogic, keyword_arguments="Optional", use_limited_api=True)
 
 %Import Qt3DCore/Qt3DCoremod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DLogic/qframeaction.sip` & `PyQt6_3D-6.7.0/sip/Qt3DLogic/qframeaction.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qframeaction.sip generated by MetaSIP
 //
 // This file is part of the Qt3DLogic Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DLogic
 {
 %TypeHeaderCode
 #include <qframeaction.h>
 %End
 
-    class QFrameAction : Qt3DCore::QComponent
+    class QFrameAction : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qframeaction.h>
 %End
 
 %ConvertToSubClassCode
         static struct class_graph {
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DLogic/qlogicaspect.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qnodraw.sip`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qlogicaspect.sip generated by MetaSIP
+// qnodraw.sip generated by MetaSIP
 //
-// This file is part of the Qt3DLogic Python extension module.
+// This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,24 +16,24 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-namespace Qt3DLogic
+namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qlogicaspect.h>
+#include <qnodraw.h>
 %End
 
-    class QLogicAspect : Qt3DCore::QAbstractAspect
+    class QNoDraw : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
-#include <qlogicaspect.h>
+#include <qnodraw.h>
 %End
 
     public:
-        explicit QLogicAspect(QObject *parent /TransferThis/ = 0);
-        virtual ~QLogicAspect();
+        explicit QNoDraw(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QNoDraw();
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/Qt3DRendermod.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/Qt3DRendermod.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Qt3DRendermod.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 
 %Import Qt3DCore/Qt3DCoremod.sip
 %Import QtCore/QtCoremod.sip
 %Import QtGui/QtGuimod.sip
 %Import QtOpenGL/QtOpenGLmod.sip
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-3D.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qabstractlight.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qabstractlight.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qabstractlight.h>
 %End
 
-    class QAbstractLight : Qt3DCore::QComponent /NoDefaultCtors/
+    class QAbstractLight : public Qt3DCore::QComponent /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qabstractlight.h>
 %End
 
     public:
         virtual ~QAbstractLight();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qabstractraycaster.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qabstractraycaster.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractraycaster.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qabstractraycaster.h>
 %End
 
-    class QAbstractRayCaster : Qt3DCore::QComponent
+    class QAbstractRayCaster : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qabstractraycaster.h>
 %End
 
     public:
         enum RunMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qabstracttexture.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qabstracttexture.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstracttexture.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qabstracttexture.h>
 %End
 
-    class QAbstractTexture : Qt3DCore::QNode
+    class QAbstractTexture : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qabstracttexture.h>
 %End
 
     public:
         enum Status
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qabstracttextureimage.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qabstracttextureimage.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstracttextureimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qabstracttextureimage.h>
 %End
 
-    class QAbstractTextureImage : Qt3DCore::QNode /Abstract/
+    class QAbstractTextureImage : public Qt3DCore::QNode /Abstract/
     {
 %TypeHeaderCode
 #include <qabstracttextureimage.h>
 %End
 
     public:
         explicit QAbstractTextureImage(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qalphacoverage.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qalphacoverage.sip`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qalphacoverage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qalphacoverage.h>
 %End
 
-    class QAlphaCoverage : Qt3DRender::QRenderState
+    class QAlphaCoverage : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qalphacoverage.h>
 %End
 
     public:
         explicit QAlphaCoverage(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qalphatest.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qalphatest.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qalphatest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qalphatest.h>
 %End
 
-    class QAlphaTest : Qt3DRender::QRenderState
+    class QAlphaTest : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qalphatest.h>
 %End
 
     public:
         enum AlphaFunction
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qblendequation.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qblendequation.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblendequation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qblendequation.h>
 %End
 
-    class QBlendEquation : Qt3DRender::QRenderState
+    class QBlendEquation : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qblendequation.h>
 %End
 
     public:
         enum BlendFunction
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qblendequationarguments.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qblendequationarguments.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblendequationarguments.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qblendequationarguments.h>
 %End
 
-    class QBlendEquationArguments : Qt3DRender::QRenderState
+    class QBlendEquationArguments : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qblendequationarguments.h>
 %End
 
     public:
         enum Blending
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qblitframebuffer.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qblitframebuffer.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qblitframebuffer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qblitframebuffer.h>
 %End
 
-    class QBlitFramebuffer : Qt3DRender::QFrameGraphNode
+    class QBlitFramebuffer : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qblitframebuffer.h>
 %End
 
     public:
         enum InterpolationMethod
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qcamera.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qcamera.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcamera.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qcamera.h>
 %End
 
-    class QCamera : Qt3DCore::QEntity
+    class QCamera : public Qt3DCore::QEntity
     {
 %TypeHeaderCode
 #include <qcamera.h>
 %End
 
 %ConvertToSubClassCode
         static struct class_graph {
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qcameralens.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qcameralens.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcameralens.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qcameralens.h>
 %End
 
-    class QCameraLens : Qt3DCore::QComponent
+    class QCameraLens : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qcameralens.h>
 %End
 
     public:
         explicit QCameraLens(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qcameraselector.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qcameraselector.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcameraselector.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qcameraselector.h>
 %End
 
-    class QCameraSelector : Qt3DRender::QFrameGraphNode
+    class QCameraSelector : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qcameraselector.h>
 %End
 
     public:
         explicit QCameraSelector(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qclearbuffers.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qclearbuffers.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclearbuffers.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qclearbuffers.h>
 %End
 
-    class QClearBuffers : Qt3DRender::QFrameGraphNode
+    class QClearBuffers : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qclearbuffers.h>
 %End
 
     public:
         explicit QClearBuffers(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qclipplane.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qclipplane.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qclipplane.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qclipplane.h>
 %End
 
-    class QClipPlane : Qt3DRender::QRenderState
+    class QClipPlane : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qclipplane.h>
 %End
 
     public:
         explicit QClipPlane(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qcolormask.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qcolormask.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcolormask.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qcolormask.h>
 %End
 
-    class QColorMask : Qt3DRender::QRenderState
+    class QColorMask : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qcolormask.h>
 %End
 
     public:
         explicit QColorMask(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qcomputecommand.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qcomputecommand.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcomputecommand.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qcomputecommand.h>
 %End
 
-    class QComputeCommand : Qt3DCore::QComponent
+    class QComputeCommand : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qcomputecommand.h>
 %End
 
     public:
         explicit QComputeCommand(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qcullface.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qcullface.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcullface.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qcullface.h>
 %End
 
-    class QCullFace : Qt3DRender::QRenderState
+    class QCullFace : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qcullface.h>
 %End
 
     public:
         enum CullingMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qdepthrange.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qdepthrange.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdepthrange.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qdepthrange.h>
 %End
 
-    class QDepthRange : Qt3DRender::QRenderState
+    class QDepthRange : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qdepthrange.h>
 %End
 
     public:
         explicit QDepthRange(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qdepthtest.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qdepthtest.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdepthtest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qdepthtest.h>
 %End
 
-    class QDepthTest : Qt3DRender::QRenderState
+    class QDepthTest : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qdepthtest.h>
 %End
 
     public:
         enum DepthFunction
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qdirectionallight.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qdirectionallight.sip`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdirectionallight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qdirectionallight.h>
 %End
 
-    class QDirectionalLight : Qt3DRender::QAbstractLight
+    class QDirectionalLight : public Qt3DRender::QAbstractLight
     {
 %TypeHeaderCode
 #include <qdirectionallight.h>
 %End
 
     public:
         explicit QDirectionalLight(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qdispatchcompute.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qdispatchcompute.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdispatchcompute.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qdispatchcompute.h>
 %End
 
-    class QDispatchCompute : Qt3DRender::QFrameGraphNode
+    class QDispatchCompute : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qdispatchcompute.h>
 %End
 
     public:
         explicit QDispatchCompute(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qdithering.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qdithering.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdithering.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qdithering.h>
 %End
 
-    class QDithering : Qt3DRender::QRenderState
+    class QDithering : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qdithering.h>
 %End
 
     public:
         explicit QDithering(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qeffect.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qeffect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qeffect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qeffect.h>
 %End
 
-    class QEffect : Qt3DCore::QNode
+    class QEffect : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qeffect.h>
 %End
 
     public:
         explicit QEffect(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qenvironmentlight.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qenvironmentlight.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qenvironmentlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qenvironmentlight.h>
 %End
 
-    class QEnvironmentLight : Qt3DCore::QComponent
+    class QEnvironmentLight : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qenvironmentlight.h>
 %End
 
     public:
         explicit QEnvironmentLight(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qfilterkey.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qfilterkey.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfilterkey.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qfilterkey.h>
 %End
 
-    class QFilterKey : Qt3DCore::QNode
+    class QFilterKey : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qfilterkey.h>
 %End
 
     public:
         explicit QFilterKey(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qframegraphnode.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qframegraphnode.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qframegraphnode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qframegraphnode.h>
 %End
 
-    class QFrameGraphNode : Qt3DCore::QNode
+    class QFrameGraphNode : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qframegraphnode.h>
 %End
 
     public:
         explicit QFrameGraphNode(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qfrontface.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qfrontface.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfrontface.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qfrontface.h>
 %End
 
-    class QFrontFace : Qt3DRender::QRenderState
+    class QFrontFace : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qfrontface.h>
 %End
 
     public:
         enum WindingDirection
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qfrustumculling.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qfrustumculling.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qfrustumculling.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qfrustumculling.h>
 %End
 
-    class QFrustumCulling : Qt3DRender::QFrameGraphNode
+    class QFrustumCulling : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qfrustumculling.h>
 %End
 
     public:
         explicit QFrustumCulling(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qgeometryrenderer.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qgeometryrenderer.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgeometryrenderer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qgeometryrenderer.h>
 %End
 
-    class QGeometryRenderer : Qt3DCore::QBoundingVolume
+    class QGeometryRenderer : public Qt3DCore::QBoundingVolume
     {
 %TypeHeaderCode
 #include <qgeometryrenderer.h>
 %End
 
     public:
         explicit QGeometryRenderer(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qgraphicsapifilter.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qgraphicsapifilter.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qgraphicsapifilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qgraphicsapifilter.h>
 %End
 
-    class QGraphicsApiFilter : QObject
+    class QGraphicsApiFilter : public QObject
     {
 %TypeHeaderCode
 #include <qgraphicsapifilter.h>
 %End
 
     public:
         enum Api
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlayer.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlayer.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlayer.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qlayer.h>
 %End
 
-    class QLayer : Qt3DCore::QComponent
+    class QLayer : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qlayer.h>
 %End
 
     public:
         explicit QLayer(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlayerfilter.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlayerfilter.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlayerfilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qlayerfilter.h>
 %End
 
-    class QLayerFilter : Qt3DRender::QFrameGraphNode
+    class QLayerFilter : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qlayerfilter.h>
 %End
 
     public:
         explicit QLayerFilter(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlevelofdetail.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlevelofdetail.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlevelofdetail.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qlevelofdetail.h>
 %End
 
-    class QLevelOfDetail : Qt3DCore::QComponent
+    class QLevelOfDetail : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qlevelofdetail.h>
 %End
 
     public:
         enum ThresholdType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlevelofdetailboundingsphere.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlevelofdetailboundingsphere.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlevelofdetailswitch.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlevelofdetailswitch.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlevelofdetailswitch.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qlevelofdetailswitch.h>
 %End
 
-    class QLevelOfDetailSwitch : Qt3DRender::QLevelOfDetail
+    class QLevelOfDetailSwitch : public Qt3DRender::QLevelOfDetail
     {
 %TypeHeaderCode
 #include <qlevelofdetailswitch.h>
 %End
 
     public:
         explicit QLevelOfDetailSwitch(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlinewidth.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlinewidth.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlinewidth.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qlinewidth.h>
 %End
 
-    class QLineWidth : Qt3DRender::QRenderState
+    class QLineWidth : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qlinewidth.h>
 %End
 
     public:
         explicit QLineWidth(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qlist.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qlist.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // This is the SIP interface definition for the QList based mapped types
 // specific to Qt3DRender.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qmaterial.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qmaterial.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmaterial.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qmaterial.h>
 %End
 
-    class QMaterial : Qt3DCore::QComponent
+    class QMaterial : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qmaterial.h>
 %End
 
     public:
         explicit QMaterial(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qmemorybarrier.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qmemorybarrier.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmemorybarrier.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qmemorybarrier.h>
 %End
 
-    class QMemoryBarrier : Qt3DRender::QFrameGraphNode
+    class QMemoryBarrier : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qmemorybarrier.h>
 %End
 
     public:
         explicit QMemoryBarrier(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qmesh.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qmesh.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmesh.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qmesh.h>
 %End
 
-    class QMesh : Qt3DRender::QGeometryRenderer
+    class QMesh : public Qt3DRender::QGeometryRenderer
     {
 %TypeHeaderCode
 #include <qmesh.h>
 %End
 
     public:
         explicit QMesh(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qmultisampleantialiasing.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qmultisampleantialiasing.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qmultisampleantialiasing.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qmultisampleantialiasing.h>
 %End
 
-    class QMultiSampleAntiAliasing : Qt3DRender::QRenderState
+    class QMultiSampleAntiAliasing : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qmultisampleantialiasing.h>
 %End
 
     public:
         explicit QMultiSampleAntiAliasing(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qnodepthmask.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qnodepthmask.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qnodepthmask.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qnodepthmask.h>
 %End
 
-    class QNoDepthMask : Qt3DRender::QRenderState
+    class QNoDepthMask : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qnodepthmask.h>
 %End
 
     public:
         explicit QNoDepthMask(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qnodraw.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qnopicking.sip`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qnodraw.sip generated by MetaSIP
+// qnopicking.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,21 +19,21 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qnodraw.h>
+#include <qnopicking.h>
 %End
 
-    class QNoDraw : Qt3DRender::QFrameGraphNode
+    class QNoPicking : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
-#include <qnodraw.h>
+#include <qnopicking.h>
 %End
 
     public:
-        explicit QNoDraw(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QNoDraw();
+        explicit QNoPicking(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QNoPicking();
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qnopicking.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpickingproxy.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qnopicking.sip generated by MetaSIP
+// qpickingproxy.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,21 +19,21 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qnopicking.h>
+#include <qpickingproxy.h>
 %End
 
-    class QNoPicking : Qt3DRender::QFrameGraphNode
+    class QPickingProxy : public Qt3DCore::QBoundingVolume
     {
 %TypeHeaderCode
-#include <qnopicking.h>
+#include <qpickingproxy.h>
 %End
 
     public:
-        explicit QNoPicking(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QNoPicking();
+        explicit QPickingProxy(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QPickingProxy();
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qobjectpicker.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qobjectpicker.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qobjectpicker.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qobjectpicker.h>
 %End
 
-    class QObjectPicker : Qt3DCore::QComponent
+    class QObjectPicker : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qobjectpicker.h>
 %End
 
     public:
         explicit QObjectPicker(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpaintedtextureimage.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpaintedtextureimage.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpaintedtextureimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpaintedtextureimage.h>
 %End
 
-    class QPaintedTextureImage : Qt3DRender::QAbstractTextureImage
+    class QPaintedTextureImage : public Qt3DRender::QAbstractTextureImage
     {
 %TypeHeaderCode
 #include <qpaintedtextureimage.h>
 %End
 
     public:
         explicit QPaintedTextureImage(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qparameter.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qparameter.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qparameter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qparameter.h>
 %End
 
-    class QParameter : Qt3DCore::QNode
+    class QParameter : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qparameter.h>
 %End
 
     public:
         explicit QParameter(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpickevent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpickevent.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpickevent.h>
 %End
 
-    class QPickEvent : QObject
+    class QPickEvent : public QObject
     {
 %TypeHeaderCode
 #include <qpickevent.h>
 %End
 
     public:
         QPickEvent();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpickingproxy.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderstate.sip`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qpickingproxy.sip generated by MetaSIP
+// qrenderstate.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,21 +19,20 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qpickingproxy.h>
+#include <qrenderstate.h>
 %End
 
-    class QPickingProxy : Qt3DCore::QBoundingVolume
+    class QRenderState : public Qt3DCore::QNode /NoDefaultCtors/
     {
 %TypeHeaderCode
-#include <qpickingproxy.h>
+#include <qrenderstate.h>
 %End
 
     public:
-        explicit QPickingProxy(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QPickingProxy();
+        virtual ~QRenderState();
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpickingsettings.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpickingsettings.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickingsettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpickingsettings.h>
 %End
 
-    class QPickingSettings : Qt3DCore::QNode
+    class QPickingSettings : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qpickingsettings.h>
 %End
 
     public:
         explicit QPickingSettings(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpicklineevent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpicklineevent.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpicklineevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpicklineevent.h>
 %End
 
-    class QPickLineEvent : Qt3DRender::QPickEvent
+    class QPickLineEvent : public Qt3DRender::QPickEvent
     {
 %TypeHeaderCode
 #include <qpicklineevent.h>
 %End
 
     public:
         QPickLineEvent();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpickpointevent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpickpointevent.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpickpointevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpickpointevent.h>
 %End
 
-    class QPickPointEvent : Qt3DRender::QPickEvent
+    class QPickPointEvent : public Qt3DRender::QPickEvent
     {
 %TypeHeaderCode
 #include <qpickpointevent.h>
 %End
 
     public:
         QPickPointEvent();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpicktriangleevent.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpicktriangleevent.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpicktriangleevent.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpicktriangleevent.h>
 %End
 
-    class QPickTriangleEvent : Qt3DRender::QPickEvent
+    class QPickTriangleEvent : public Qt3DRender::QPickEvent
     {
 %TypeHeaderCode
 #include <qpicktriangleevent.h>
 %End
 
     public:
         QPickTriangleEvent();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpointlight.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpointlight.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpointlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpointlight.h>
 %End
 
-    class QPointLight : Qt3DRender::QAbstractLight
+    class QPointLight : public Qt3DRender::QAbstractLight
     {
 %TypeHeaderCode
 #include <qpointlight.h>
 %End
 
     public:
         explicit QPointLight(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpointsize.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpointsize.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpointsize.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpointsize.h>
 %End
 
-    class QPointSize : Qt3DRender::QRenderState
+    class QPointSize : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qpointsize.h>
 %End
 
     public:
         enum SizeMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qpolygonoffset.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qpolygonoffset.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpolygonoffset.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qpolygonoffset.h>
 %End
 
-    class QPolygonOffset : Qt3DRender::QRenderState
+    class QPolygonOffset : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qpolygonoffset.h>
 %End
 
     public:
         explicit QPolygonOffset(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qproximityfilter.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qproximityfilter.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qproximityfilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qproximityfilter.h>
 %End
 
-    class QProximityFilter : Qt3DRender::QFrameGraphNode
+    class QProximityFilter : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qproximityfilter.h>
 %End
 
     public:
         explicit QProximityFilter(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrastermode.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrastermode.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrastermode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrastermode.h>
 %End
 
-    class QRasterMode : Qt3DRender::QRenderState
+    class QRasterMode : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qrastermode.h>
 %End
 
     public:
         enum RasterMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qraycaster.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qraycaster.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qraycaster.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qraycaster.h>
 %End
 
-    class QRayCaster : Qt3DRender::QAbstractRayCaster
+    class QRayCaster : public Qt3DRender::QAbstractRayCaster
     {
 %TypeHeaderCode
 #include <qraycaster.h>
 %End
 
     public:
         explicit QRayCaster(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qraycasterhit.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qraycasterhit.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qraycasterhit.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderapi.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderapi.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderapi.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderaspect.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderaspect.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderaspect.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -29,15 +29,15 @@
     namespace Render
     {
 %TypeHeaderCode
 #include <qrenderaspect.h>
 %End
     };
 
-    class QRenderAspect : Qt3DCore::QAbstractAspect
+    class QRenderAspect : public Qt3DCore::QAbstractAspect
     {
 %TypeHeaderCode
 #include <qrenderaspect.h>
 %End
 
     public:
         enum SubmissionType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendercapabilities.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendercapabilities.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendercapabilities.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrendercapabilities.h>
 %End
 
-    class QRenderCapabilities : QObject
+    class QRenderCapabilities : public QObject
     {
 %TypeHeaderCode
 #include <qrendercapabilities.h>
 %End
 
     public:
         enum API
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendercapture.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendercapture.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendercapture.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrendercapture.h>
 %End
 
-    class QRenderCaptureReply : QObject
+    class QRenderCaptureReply : public QObject
     {
 %TypeHeaderCode
 #include <qrendercapture.h>
 %End
 
     public:
         QImage image() const;
@@ -40,15 +40,15 @@
     signals:
         void completed();
 
     private:
         QRenderCaptureReply(QObject *parent /TransferThis/ = 0);
     };
 
-    class QRenderCapture : Qt3DRender::QFrameGraphNode
+    class QRenderCapture : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qrendercapture.h>
 %End
 
     public:
         explicit QRenderCapture(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderpass.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderpass.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderpass.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrenderpass.h>
 %End
 
-    class QRenderPass : Qt3DCore::QNode
+    class QRenderPass : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qrenderpass.h>
 %End
 
     public:
         explicit QRenderPass(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderpassfilter.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderpassfilter.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrenderpassfilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrenderpassfilter.h>
 %End
 
-    class QRenderPassFilter : Qt3DRender::QFrameGraphNode
+    class QRenderPassFilter : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qrenderpassfilter.h>
 %End
 
     public:
         explicit QRenderPassFilter(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendersettings.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendersettings.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendersettings.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrendersettings.h>
 %End
 
-    class QRenderSettings : Qt3DCore::QComponent
+    class QRenderSettings : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qrendersettings.h>
 %End
 
     public:
         explicit QRenderSettings(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderstate.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrenderstateset.sip`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qrenderstate.sip generated by MetaSIP
+// qrenderstateset.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,20 +19,32 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qrenderstate.h>
+#include <qrenderstateset.h>
 %End
 
-    class QRenderState : Qt3DCore::QNode /NoDefaultCtors/
+    class QRenderStateSet : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
-#include <qrenderstate.h>
+#include <qrenderstateset.h>
 %End
 
     public:
-        virtual ~QRenderState();
+        explicit QRenderStateSet(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QRenderStateSet();
+        void addRenderState(Qt3DRender::QRenderState *state /GetWrapper/);
+%MethodCode
+            // This takes ownership only if it doesn't already have a parent.
+            if (!a0->parent())
+                sipTransferTo(a0Wrapper, sipSelf);
+            
+            sipCpp->addRenderState(a0);
+%End
+
+        void removeRenderState(Qt3DRender::QRenderState *state);
+        QList<Qt3DRender::QRenderState *> renderStates() const;
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrenderstateset.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendertargetselector.sip`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qrenderstateset.sip generated by MetaSIP
+// qrendertargetselector.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,32 +19,28 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qrenderstateset.h>
+#include <qrendertargetselector.h>
 %End
 
-    class QRenderStateSet : Qt3DRender::QFrameGraphNode
+    class QRenderTargetSelector : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
-#include <qrenderstateset.h>
+#include <qrendertargetselector.h>
 %End
 
     public:
-        explicit QRenderStateSet(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QRenderStateSet();
-        void addRenderState(Qt3DRender::QRenderState *state /GetWrapper/);
-%MethodCode
-            // This takes ownership only if it doesn't already have a parent.
-            if (!a0->parent())
-                sipTransferTo(a0Wrapper, sipSelf);
-            
-            sipCpp->addRenderState(a0);
-%End
+        explicit QRenderTargetSelector(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QRenderTargetSelector();
+        Qt3DRender::QRenderTarget *target() const;
+
+    public slots:
+        void setTarget(Qt3DRender::QRenderTarget *target);
 
-        void removeRenderState(Qt3DRender::QRenderState *state);
-        QList<Qt3DRender::QRenderState *> renderStates() const;
+    signals:
+        void targetChanged(Qt3DRender::QRenderTarget *target /ScopesStripped=1/);
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendersurfaceselector.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendersurfaceselector.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendersurfaceselector.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrendersurfaceselector.h>
 %End
 
-    class QRenderSurfaceSelector : Qt3DRender::QFrameGraphNode
+    class QRenderSurfaceSelector : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qrendersurfaceselector.h>
 %End
 
     public:
         explicit QRenderSurfaceSelector(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendertarget.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendertarget.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendertarget.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrendertarget.h>
 %End
 
-    class QRenderTarget : Qt3DCore::QComponent
+    class QRenderTarget : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qrendertarget.h>
 %End
 
     public:
         explicit QRenderTarget(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendertargetoutput.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qrendertargetoutput.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qrendertargetoutput.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qrendertargetoutput.h>
 %End
 
-    class QRenderTargetOutput : Qt3DCore::QNode
+    class QRenderTargetOutput : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qrendertargetoutput.h>
 %End
 
     public:
         enum AttachmentPoint
@@ -50,14 +50,20 @@
             Color12,
             Color13,
             Color14,
             Color15,
             Depth,
             Stencil,
             DepthStencil,
+%If (Qt3D_6_7_0 -)
+            Left,
+%End
+%If (Qt3D_6_7_0 -)
+            Right,
+%End
         };
 
         explicit QRenderTargetOutput(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QRenderTargetOutput();
         Qt3DRender::QRenderTargetOutput::AttachmentPoint attachmentPoint() const;
         Qt3DRender::QAbstractTexture *texture() const;
         int mipLevel() const;
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qrendertargetselector.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciltest.sip`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qrendertargetselector.sip generated by MetaSIP
+// qstenciltest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,28 +19,23 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qrendertargetselector.h>
+#include <qstenciltest.h>
 %End
 
-    class QRenderTargetSelector : Qt3DRender::QFrameGraphNode
+    class QStencilTest : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
-#include <qrendertargetselector.h>
+#include <qstenciltest.h>
 %End
 
     public:
-        explicit QRenderTargetSelector(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QRenderTargetSelector();
-        Qt3DRender::QRenderTarget *target() const;
-
-    public slots:
-        void setTarget(Qt3DRender::QRenderTarget *target);
-
-    signals:
-        void targetChanged(Qt3DRender::QRenderTarget *target /ScopesStripped=1/);
+        explicit QStencilTest(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QStencilTest();
+        Qt3DRender::QStencilTestArguments *front() const;
+        Qt3DRender::QStencilTestArguments *back() const;
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qsceneloader.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qsceneloader.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsceneloader.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qsceneloader.h>
 %End
 
-    class QSceneLoader : Qt3DCore::QComponent
+    class QSceneLoader : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qsceneloader.h>
 %End
 
     public:
         explicit QSceneLoader(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qscissortest.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qscissortest.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscissortest.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qscissortest.h>
 %End
 
-    class QScissorTest : Qt3DRender::QRenderState
+    class QScissorTest : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qscissortest.h>
 %End
 
     public:
         explicit QScissorTest(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qscreenraycaster.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qscreenraycaster.sip`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscreenraycaster.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qscreenraycaster.h>
 %End
 
-    class QScreenRayCaster : Qt3DRender::QAbstractRayCaster
+    class QScreenRayCaster : public Qt3DRender::QAbstractRayCaster
     {
 %TypeHeaderCode
 #include <qscreenraycaster.h>
 %End
 
     public:
         explicit QScreenRayCaster(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qseamlesscubemap.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qseamlesscubemap.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qseamlesscubemap.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qseamlesscubemap.h>
 %End
 
-    class QSeamlessCubemap : Qt3DRender::QRenderState
+    class QSeamlessCubemap : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qseamlesscubemap.h>
 %End
 
     public:
         explicit QSeamlessCubemap(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qsetfence.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qsetfence.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsetfence.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qsetfence.h>
 %End
 
-    class QSetFence : Qt3DRender::QFrameGraphNode
+    class QSetFence : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qsetfence.h>
 %End
 
     public:
         enum HandleType
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderdata.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderdata.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderdata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -35,15 +35,15 @@
     public:
         virtual ~PropertyReaderInterface();
         virtual QVariant readProperty(const QVariant &v) = 0;
     };
 
     typedef QSharedPointer<Qt3DRender::PropertyReaderInterface> PropertyReaderInterfacePtr;
 
-    class QShaderData : Qt3DCore::QComponent
+    class QShaderData : public Qt3DCore::QComponent
     {
 %TypeHeaderCode
 #include <qshaderdata.h>
 %End
 
     public:
         explicit QShaderData(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderimage.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderimage.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qshaderimage.h>
 %End
 
-    class QShaderImage : Qt3DCore::QNode
+    class QShaderImage : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qshaderimage.h>
 %End
 
     public:
         enum Access
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderprogram.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderprogram.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderprogram.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qshaderprogram.h>
 %End
 
-    class QShaderProgram : Qt3DCore::QNode
+    class QShaderProgram : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qshaderprogram.h>
 %End
 
     public:
         explicit QShaderProgram(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qshaderprogrambuilder.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qshaderprogrambuilder.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qshaderprogrambuilder.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qshaderprogrambuilder.h>
 %End
 
-    class QShaderProgramBuilder : Qt3DCore::QNode
+    class QShaderProgramBuilder : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qshaderprogrambuilder.h>
 %End
 
     public:
         explicit QShaderProgramBuilder(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qsortpolicy.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qsortpolicy.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsortpolicy.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qsortpolicy.h>
 %End
 
-    class QSortPolicy : Qt3DRender::QFrameGraphNode
+    class QSortPolicy : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qsortpolicy.h>
 %End
 
     public:
         explicit QSortPolicy(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qspotlight.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qspotlight.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qspotlight.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qspotlight.h>
 %End
 
-    class QSpotLight : Qt3DRender::QAbstractLight
+    class QSpotLight : public Qt3DRender::QAbstractLight
     {
 %TypeHeaderCode
 #include <qspotlight.h>
 %End
 
     public:
         explicit QSpotLight(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qstencilmask.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qstencilmask.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstencilmask.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qstencilmask.h>
 %End
 
-    class QStencilMask : Qt3DRender::QRenderState
+    class QStencilMask : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qstencilmask.h>
 %End
 
     public:
         explicit QStencilMask(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciloperation.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciloperation.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciloperation.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qstenciloperation.h>
 %End
 
-    class QStencilOperation : Qt3DRender::QRenderState
+    class QStencilOperation : public Qt3DRender::QRenderState
     {
 %TypeHeaderCode
 #include <qstenciloperation.h>
 %End
 
     public:
         explicit QStencilOperation(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciloperationarguments.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciloperationarguments.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciloperationarguments.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qstenciloperationarguments.h>
 %End
 
-    class QStencilOperationArguments : QObject /NoDefaultCtors/
+    class QStencilOperationArguments : public QObject /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qstenciloperationarguments.h>
 %End
 
     public:
         enum FaceMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciltest.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qviewport.sip`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qstenciltest.sip generated by MetaSIP
+// qviewport.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,23 +19,37 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qstenciltest.h>
+#include <qviewport.h>
 %End
 
-    class QStencilTest : Qt3DRender::QRenderState
+    class QViewport : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
-#include <qstenciltest.h>
+#include <qviewport.h>
 %End
 
     public:
-        explicit QStencilTest(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QStencilTest();
-        Qt3DRender::QStencilTestArguments *front() const;
-        Qt3DRender::QStencilTestArguments *back() const;
+        explicit QViewport(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QViewport();
+        QRectF normalizedRect() const;
+
+    public slots:
+        void setNormalizedRect(const QRectF &normalizedRect);
+
+    signals:
+        void normalizedRectChanged(const QRectF &normalizedRect);
+
+    public:
+        float gamma() const;
+
+    public slots:
+        void setGamma(float gamma);
+
+    signals:
+        void gammaChanged(float gamma);
     };
 };
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qstenciltestarguments.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qstenciltestarguments.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstenciltestarguments.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qstenciltestarguments.h>
 %End
 
-    class QStencilTestArguments : QObject /NoDefaultCtors/
+    class QStencilTestArguments : public QObject /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qstenciltestarguments.h>
 %End
 
     public:
         enum StencilFaceMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qsubtreeenabler.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qsubtreeenabler.sip`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsubtreeenabler.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qsubtreeenabler.h>
 %End
 
-    class QSubtreeEnabler : Qt3DRender::QFrameGraphNode
+    class QSubtreeEnabler : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qsubtreeenabler.h>
 %End
 
     public:
         explicit QSubtreeEnabler(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtechnique.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtechnique.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtechnique.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qtechnique.h>
 %End
 
-    class QTechnique : Qt3DCore::QNode
+    class QTechnique : public Qt3DCore::QNode
     {
 %TypeHeaderCode
 #include <qtechnique.h>
 %End
 
     public:
         explicit QTechnique(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtechniquefilter.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtechniquefilter.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtechniquefilter.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qtechniquefilter.h>
 %End
 
-    class QTechniqueFilter : Qt3DRender::QFrameGraphNode
+    class QTechniqueFilter : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
 #include <qtechniquefilter.h>
 %End
 
     public:
         explicit QTechniqueFilter(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtexture.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtexture.sip`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexture.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,136 +22,136 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
-    class QTexture1D : Qt3DRender::QAbstractTexture
+    class QTexture1D : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture1D(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture1D();
     };
 
-    class QTexture1DArray : Qt3DRender::QAbstractTexture
+    class QTexture1DArray : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture1DArray(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture1DArray();
     };
 
-    class QTexture2D : Qt3DRender::QAbstractTexture
+    class QTexture2D : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture2D(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture2D();
     };
 
-    class QTexture2DArray : Qt3DRender::QAbstractTexture
+    class QTexture2DArray : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture2DArray(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture2DArray();
     };
 
-    class QTexture3D : Qt3DRender::QAbstractTexture
+    class QTexture3D : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture3D(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture3D();
     };
 
-    class QTextureCubeMap : Qt3DRender::QAbstractTexture
+    class QTextureCubeMap : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTextureCubeMap(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTextureCubeMap();
     };
 
-    class QTextureCubeMapArray : Qt3DRender::QAbstractTexture
+    class QTextureCubeMapArray : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTextureCubeMapArray(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTextureCubeMapArray();
     };
 
-    class QTexture2DMultisample : Qt3DRender::QAbstractTexture
+    class QTexture2DMultisample : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture2DMultisample(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture2DMultisample();
     };
 
-    class QTexture2DMultisampleArray : Qt3DRender::QAbstractTexture
+    class QTexture2DMultisampleArray : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTexture2DMultisampleArray(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTexture2DMultisampleArray();
     };
 
-    class QTextureRectangle : Qt3DRender::QAbstractTexture
+    class QTextureRectangle : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTextureRectangle(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTextureRectangle();
     };
 
-    class QTextureBuffer : Qt3DRender::QAbstractTexture
+    class QTextureBuffer : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTextureBuffer(Qt3DCore::QNode *parent /TransferThis/ = 0);
         virtual ~QTextureBuffer();
     };
 
-    class QTextureLoader : Qt3DRender::QAbstractTexture
+    class QTextureLoader : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QTextureLoader(Qt3DCore::QNode *parent /TransferThis/ = 0);
@@ -170,15 +170,15 @@
     public slots:
         void setMirrored(bool mirrored);
 
     signals:
         void mirroredChanged(bool mirrored);
     };
 
-    class QSharedGLTexture : Qt3DRender::QAbstractTexture
+    class QSharedGLTexture : public Qt3DRender::QAbstractTexture
     {
 %TypeHeaderCode
 #include <qtexture.h>
 %End
 
     public:
         explicit QSharedGLTexture(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtexturedata.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtexturedata.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturedata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtexturedataupdate.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtexturedataupdate.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturedataupdate.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtextureimage.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtextureimage.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtextureimage.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qtextureimage.h>
 %End
 
-    class QTextureImage : Qt3DRender::QAbstractTextureImage
+    class QTextureImage : public Qt3DRender::QAbstractTextureImage
     {
 %TypeHeaderCode
 #include <qtextureimage.h>
 %End
 
     public:
         explicit QTextureImage(Qt3DCore::QNode *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtextureimagedata.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtextureimagedata.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtextureimagedata.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtextureimagedatagenerator.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtextureimagedatagenerator.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtextureimagedatagenerator.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -24,15 +24,15 @@
 {
 %TypeHeaderCode
 #include <qtextureimagedatagenerator.h>
 %End
 
     typedef QSharedPointer<Qt3DRender::QTextureImageDataGenerator> QTextureImageDataGeneratorPtr;
 
-    class QTextureImageDataGenerator : Qt3DCore::QAbstractFunctor /NoDefaultCtors/
+    class QTextureImageDataGenerator : public Qt3DCore::QAbstractFunctor /NoDefaultCtors/
     {
 %TypeHeaderCode
 #include <qtextureimagedatagenerator.h>
 %End
 
     public:
         virtual ~QTextureImageDataGenerator();
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qtexturewrapmode.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qtexturewrapmode.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qtexturewrapmode.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -22,15 +22,15 @@
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
 #include <qtexturewrapmode.h>
 %End
 
-    class QTextureWrapMode : QObject
+    class QTextureWrapMode : public QObject
     {
 %TypeHeaderCode
 #include <qtexturewrapmode.h>
 %End
 
     public:
         enum WrapMode
```

### Comparing `PyQt6_3D-6.6.0/sip/Qt3DRender/qviewport.sip` & `PyQt6_3D-6.7.0/sip/Qt3DRender/qwaitfence.sip`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-// qviewport.sip generated by MetaSIP
+// qwaitfence.sip generated by MetaSIP
 //
 // This file is part of the Qt3DRender Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-3D.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -19,37 +19,41 @@
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 namespace Qt3DRender
 {
 %TypeHeaderCode
-#include <qviewport.h>
+#include <qwaitfence.h>
 %End
 
-    class QViewport : Qt3DRender::QFrameGraphNode
+    class QWaitFence : public Qt3DRender::QFrameGraphNode
     {
 %TypeHeaderCode
-#include <qviewport.h>
+#include <qwaitfence.h>
 %End
 
     public:
-        explicit QViewport(Qt3DCore::QNode *parent /TransferThis/ = 0);
-        virtual ~QViewport();
-        QRectF normalizedRect() const;
-
-    public slots:
-        void setNormalizedRect(const QRectF &normalizedRect);
-
-    signals:
-        void normalizedRectChanged(const QRectF &normalizedRect);
-
-    public:
-        float gamma() const;
-
-    public slots:
-        void setGamma(float gamma);
+        enum HandleType
+        {
+            NoHandle,
+            OpenGLFenceId,
+        };
+
+        explicit QWaitFence(Qt3DCore::QNode *parent /TransferThis/ = 0);
+        virtual ~QWaitFence();
+        void setHandleType(Qt3DRender::QWaitFence::HandleType type);
+        void setHandle(QVariant handle);
+        Qt3DRender::QWaitFence::HandleType handleType() const;
+        QVariant handle() const;
+        bool waitOnCPU() const;
+        void setWaitOnCPU(bool waitOnCPU);
+        quint64 timeout() const;
+        void setTimeout(quint64 timeout);
 
     signals:
-        void gammaChanged(float gamma);
+        void waitOnCPUChanged(bool waitOnCPU);
+        void timeoutChanged(quint64 timeoutChanged);
+        void handleTypeChanged(Qt3DRender::QWaitFence::HandleType handleType);
+        void handleChanged(QVariant handle);
     };
 };
```

