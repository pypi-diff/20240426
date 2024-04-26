# Comparing `tmp/KratosMultiphysics_all-9.4.5-py3-none-any.whl.zip` & `tmp/KratosMultiphysics_all-9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 5198 bytes, number of entries: 4
--rw-r--r--  2.0 unx    12763 b- defN 24-Jan-09 14:16 KratosMultiphysics_all-9.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-09 14:16 KratosMultiphysics_all-9.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Jan-09 14:16 KratosMultiphysics_all-9.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      359 b- defN 24-Jan-09 14:16 KratosMultiphysics_all-9.4.5.dist-info/RECORD
-4 files, 13233 bytes uncompressed, 4496 bytes compressed:  66.0%
+Zip file size: 5232 bytes, number of entries: 4
+-rw-r--r--  2.0 unx    12835 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      351 b- defN 24-Apr-25 16:37 KratosMultiphysics_all-9.5.dist-info/RECORD
+4 files, 13297 bytes uncompressed, 4546 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: KratosMultiphysics_all-9.4.5.dist-info/METADATA
+Filename: KratosMultiphysics_all-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics_all-9.4.5.dist-info/WHEEL
+Filename: KratosMultiphysics_all-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics_all-9.4.5.dist-info/top_level.txt
+Filename: KratosMultiphysics_all-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics_all-9.4.5.dist-info/RECORD
+Filename: KratosMultiphysics_all-9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `KratosMultiphysics_all-9.4.5.dist-info/METADATA` & `KratosMultiphysics_all-9.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KratosMultiphysics-all
-Version: 9.4.5
+Version: 9.5
 Summary: KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface.
 Home-page: https://github.com/KratosMultiphysics/
 Author: Kratos Team
 Author-email: kratos@listas.cimne.upc.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
@@ -20,45 +20,45 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: KratosMultiphysics (==9.4.5)
-Requires-Dist: KratosContactStructuralMechanicsApplication (==9.4.5)
-Requires-Dist: KratosConvectionDiffusionApplication (==9.4.5)
-Requires-Dist: KratosConstitutiveLawsApplication (==9.4.5)
-Requires-Dist: KratosCoSimulationApplication (==9.4.5)
-Requires-Dist: KratosDEMApplication (==9.4.5)
-Requires-Dist: KratosDamApplication (==9.4.5)
-Requires-Dist: KratosFluidDynamicsApplication (==9.4.5)
-Requires-Dist: KratosFSIApplication (==9.4.5)
-Requires-Dist: KratosLinearSolversApplication (==9.4.5)
-Requires-Dist: KratosMappingApplication (==9.4.5)
-Requires-Dist: KratosMeshingApplication (==9.4.5)
-Requires-Dist: KratosParticleMechanicsApplication (==9.4.5)
-Requires-Dist: KratosPoroMechanicsApplication (==9.4.5)
-Requires-Dist: KratosShallowWaterApplication (==9.4.5)
-Requires-Dist: KratosStructuralMechanicsApplication (==9.4.5)
-Requires-Dist: KratosGeoMechanicsApplication (==9.4.5)
+Requires-Dist: KratosMultiphysics ==9.5
+Requires-Dist: KratosContactStructuralMechanicsApplication ==9.5
+Requires-Dist: KratosConvectionDiffusionApplication ==9.5
+Requires-Dist: KratosConstitutiveLawsApplication ==9.5
+Requires-Dist: KratosCoSimulationApplication ==9.5
+Requires-Dist: KratosDEMApplication ==9.5
+Requires-Dist: KratosDamApplication ==9.5
+Requires-Dist: KratosFluidDynamicsApplication ==9.5
+Requires-Dist: KratosFSIApplication ==9.5
+Requires-Dist: KratosLinearSolversApplication ==9.5
+Requires-Dist: KratosMappingApplication ==9.5
+Requires-Dist: KratosMeshingApplication ==9.5
+Requires-Dist: KratosMPMApplication ==9.5
+Requires-Dist: KratosPoroMechanicsApplication ==9.5
+Requires-Dist: KratosShallowWaterApplication ==9.5
+Requires-Dist: KratosStructuralMechanicsApplication ==9.5
+Requires-Dist: KratosGeoMechanicsApplication ==9.5
 
 <p align=center><img height="72.125%" width="72.125%" src="https://raw.githubusercontent.com/KratosMultiphysics/Documentation/master/Wiki_files/Home/kratos.png"></p>
 
-[![License][license-image]][license] [![C++][c++-image]][c++standard] [![Github CI][Nightly-Build]][Nightly-link] [![DOI][DOI-image]][DOI] [![GitHub stars][stars-image]][stars] [![Twitter][twitter-image]][twitter]
+[![License][license-image]][license] [![C++][c++-image]][c++standard] [![Github CI][Nightly-Build]][Nightly-link] [![DOI][DOI-image]][DOI] [![GitHub stars][stars-image]][stars] [![Twitter][twitter-image]][twitter] [![Youtube][youtube-image]][youtube]
 
 [![Release][release-image]][releases]
 <a href="https://github.com/KratosMultiphysics/Kratos/releases/latest"><img src="https://img.shields.io/github/release-date/KratosMultiphysics/Kratos?label="></a>
 <a href="https://github.com/KratosMultiphysics/Kratos/compare/Release-8.1...master"><img src="https://img.shields.io/github/commits-since/KratosMultiphysics/Kratos/latest?label=commits%20since"></a>
 <a href="https://github.com/KratosMultiphysics/Kratos/commit/master"><img src="https://img.shields.io/github/last-commit/KratosMultiphysics/Kratos?label=latest%20commit"></a>
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/KratosMultiphysics.svg)](https://pypi.org/project/KratosMultiphysics/)
 [![Downloads](https://pepy.tech/badge/KratosMultiphysics/month)](https://pepy.tech/project/KratosMultiphysics)
 
-[release-image]: https://img.shields.io/badge/release-9.3-green.svg?style=flat
+[release-image]: https://img.shields.io/badge/release-9.4-green.svg?style=flat
 [releases]: https://github.com/KratosMultiphysics/Kratos/releases
 
 [license-image]: https://img.shields.io/badge/license-BSD-green.svg?style=flat
 [license]: https://github.com/KratosMultiphysics/Kratos/blob/master/kratos/license.txt
 
 [c++-image]: https://img.shields.io/badge/C++-17-blue.svg?style=flat&logo=c%2B%2B
 [c++standard]: https://isocpp.org/std/the-standard
@@ -71,14 +71,17 @@
 
 [stars-image]: https://img.shields.io/github/stars/KratosMultiphysics/Kratos?label=Stars&logo=github
 [stars]: https://github.com/KratosMultiphysics/Kratos/stargazers
 
 [twitter-image]: https://img.shields.io/twitter/follow/kratosmultiphys.svg?label=Follow&style=social
 [twitter]: https://twitter.com/kratosmultiphys
 
+[youtube-image]: https://badges.aleen42.com/src/youtube.svg
+[youtube]:https://www.youtube.com/@kratosmultiphysics3578
+
 _KRATOS Multiphysics_ ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface. More in [Overview](https://github.com/KratosMultiphysics/Kratos/wiki/Overview)
 
 **Kratos** is **free** under BSD-4 [license](https://github.com/KratosMultiphysics/Kratos/wiki/Licence) and can be used even in comercial softwares as it is. Many of its main applications are also free and BSD-4 licensed but each derived application can have its own propietary license.
 
 # Main Features
 **Kratos** is __multiplatform__ and available for __Windows, Linux__ (several distros) and __macOS__.
```

### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: KratosMultiphysics-all Version: 9.4.5 Summary:
-KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-
+Metadata-Version: 2.1 Name: KratosMultiphysics-all Version: 9.5 Summary: KRATOS
+Multiphysics ("Kratos") is a framework for building parallel, multi-
 disciplinary simulation software, aiming at modularity, extensibility, and high
 performance. Kratos is written in C++, and counts with an extensive Python
 interface. Home-page: https://github.com/KratosMultiphysics/ Author: Kratos
 Team Author-email: kratos@listas.cimne.upc.edu Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -11,77 +11,78 @@
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Physics Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: License :: OSI Approved :: BSD License Classifier:
 Natural Language :: English Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Other Audience Classifier: Intended Audience
 :: Developers Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Requires-Python: >=3.8 Description-Content-
-Type: text/markdown Requires-Dist: KratosMultiphysics (==9.4.5) Requires-Dist:
-KratosContactStructuralMechanicsApplication (==9.4.5) Requires-Dist:
-KratosConvectionDiffusionApplication (==9.4.5) Requires-Dist:
-KratosConstitutiveLawsApplication (==9.4.5) Requires-Dist:
-KratosCoSimulationApplication (==9.4.5) Requires-Dist: KratosDEMApplication
-(==9.4.5) Requires-Dist: KratosDamApplication (==9.4.5) Requires-Dist:
-KratosFluidDynamicsApplication (==9.4.5) Requires-Dist: KratosFSIApplication
-(==9.4.5) Requires-Dist: KratosLinearSolversApplication (==9.4.5) Requires-
-Dist: KratosMappingApplication (==9.4.5) Requires-Dist:
-KratosMeshingApplication (==9.4.5) Requires-Dist:
-KratosParticleMechanicsApplication (==9.4.5) Requires-Dist:
-KratosPoroMechanicsApplication (==9.4.5) Requires-Dist:
-KratosShallowWaterApplication (==9.4.5) Requires-Dist:
-KratosStructuralMechanicsApplication (==9.4.5) Requires-Dist:
-KratosGeoMechanicsApplication (==9.4.5)
+Type: text/markdown Requires-Dist: KratosMultiphysics ==9.5 Requires-Dist:
+KratosContactStructuralMechanicsApplication ==9.5 Requires-Dist:
+KratosConvectionDiffusionApplication ==9.5 Requires-Dist:
+KratosConstitutiveLawsApplication ==9.5 Requires-Dist:
+KratosCoSimulationApplication ==9.5 Requires-Dist: KratosDEMApplication ==9.5
+Requires-Dist: KratosDamApplication ==9.5 Requires-Dist:
+KratosFluidDynamicsApplication ==9.5 Requires-Dist: KratosFSIApplication ==9.5
+Requires-Dist: KratosLinearSolversApplication ==9.5 Requires-Dist:
+KratosMappingApplication ==9.5 Requires-Dist: KratosMeshingApplication ==9.5
+Requires-Dist: KratosMPMApplication ==9.5 Requires-Dist:
+KratosPoroMechanicsApplication ==9.5 Requires-Dist:
+KratosShallowWaterApplication ==9.5 Requires-Dist:
+KratosStructuralMechanicsApplication ==9.5 Requires-Dist:
+KratosGeoMechanicsApplication ==9.5
   [https://raw.githubusercontent.com/KratosMultiphysics/Documentation/master/
                           Wiki_files/Home/kratos.png]
 [![License][license-image]][license] [![C++][c++-image]][c++standard] [![Github
 CI][Nightly-Build]][Nightly-link] [![DOI][DOI-image]][DOI] [![GitHub stars]
-[stars-image]][stars] [![Twitter][twitter-image]][twitter] [![Release][release-
-image]][releases] _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_-_d_a_t_e_/
-_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_?_l_a_b_e_l_=_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_m_m_i_t_s_-_s_i_n_c_e_/
-_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_/_l_a_t_e_s_t_?_l_a_b_e_l_=_c_o_m_m_i_t_s_%_2_0_s_i_n_c_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_?_l_a_b_e_l_=_l_a_t_e_s_t_%_2_0_c_o_m_m_i_t_][![PyPI
-pyversions](https://img.shields.io/pypi/pyversions/KratosMultiphysics.svg)]
-(https://pypi.org/project/KratosMultiphysics/) [![Downloads](https://pepy.tech/
-badge/KratosMultiphysics/month)](https://pepy.tech/project/KratosMultiphysics)
-[release-image]: https://img.shields.io/badge/release-9.3-green.svg?style=flat
-[releases]: https://github.com/KratosMultiphysics/Kratos/releases [license-
-image]: https://img.shields.io/badge/license-BSD-green.svg?style=flat
-[license]: https://github.com/KratosMultiphysics/Kratos/blob/master/kratos/
-license.txt [c++-image]: https://img.shields.io/badge/C++-17-
-blue.svg?style=flat&logo=c%2B%2B [c++standard]: https://isocpp.org/std/the-
-standard [Nightly-Build]: https://github.com/KratosMultiphysics/Kratos/
-workflows/Nightly%20Build/badge.svg [Nightly-link]: https://github.com/
-KratosMultiphysics/Kratos/actions?query=workflow%3A%22Nightly+Build%22 [DOI-
-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.3234644.svg [DOI]: https://
-doi.org/10.5281/zenodo.3234644 [stars-image]: https://img.shields.io/github/
-stars/KratosMultiphysics/Kratos?label=Stars&logo=github [stars]: https://
-github.com/KratosMultiphysics/Kratos/stargazers [twitter-image]: https://
-img.shields.io/twitter/follow/kratosmultiphys.svg?label=Follow&style=social
-[twitter]: https://twitter.com/kratosmultiphys _KRATOS Multiphysics_ ("Kratos")
-is a framework for building parallel, multi-disciplinary simulation software,
-aiming at modularity, extensibility, and high performance. Kratos is written in
-C++, and counts with an extensive Python interface. More in [Overview](https://
-github.com/KratosMultiphysics/Kratos/wiki/Overview) **Kratos** is **free**
-under BSD-4 [license](https://github.com/KratosMultiphysics/Kratos/wiki/
-Licence) and can be used even in comercial softwares as it is. Many of its main
-applications are also free and BSD-4 licensed but each derived application can
-have its own propietary license. # Main Features **Kratos** is
-__multiplatform__ and available for __Windows, Linux__ (several distros) and
-__macOS__. **Kratos** is __OpenMP__ and __MPI__ parallel and scalable up to
-thousands of cores. **Kratos** provides a core which defines the common
-framework and several application which work like plug-ins that can be extended
-in diverse fields. ## Its main applications are: - [DEM](applications/
-DEMApplication) for cohesive and non cohesive spheric and non spheric particles
-simulation - [Fluid Dynamics](applications/FluidDynamicsApplication/README.md)
-Provides 2D and 3D incompressible fluids formulation - [Fluid Structure
-Interaction](applications/FSIApplication/README.md) for solution of different
-FSI problems - [Structural Mechanics](applications/
-StructuralMechanicsApplication/README.md) Providing solution for solid, shell
-and beam structures with linear and nonlinear, static and dynamic behavior -
-[Contact Structural Mechanics](applications/
+[stars-image]][stars] [![Twitter][twitter-image]][twitter] [![Youtube][youtube-
+image]][youtube] [![Release][release-image]][releases] _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_g_i_t_h_u_b_/_r_e_l_e_a_s_e_-_d_a_t_e_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_?_l_a_b_e_l_=_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+_g_i_t_h_u_b_/_c_o_m_m_i_t_s_-_s_i_n_c_e_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/_K_r_a_t_o_s_/_l_a_t_e_s_t_?_l_a_b_e_l_=_c_o_m_m_i_t_s_%_2_0_s_i_n_c_e_]
+_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_a_s_t_-_c_o_m_m_i_t_/_K_r_a_t_o_s_M_u_l_t_i_p_h_y_s_i_c_s_/
+_K_r_a_t_o_s_?_l_a_b_e_l_=_l_a_t_e_s_t_%_2_0_c_o_m_m_i_t_][![PyPI pyversions](https://img.shields.io/pypi/
+pyversions/KratosMultiphysics.svg)](https://pypi.org/project/
+KratosMultiphysics/) [![Downloads](https://pepy.tech/badge/KratosMultiphysics/
+month)](https://pepy.tech/project/KratosMultiphysics) [release-image]: https://
+img.shields.io/badge/release-9.4-green.svg?style=flat [releases]: https://
+github.com/KratosMultiphysics/Kratos/releases [license-image]: https://
+img.shields.io/badge/license-BSD-green.svg?style=flat [license]: https://
+github.com/KratosMultiphysics/Kratos/blob/master/kratos/license.txt [c++-
+image]: https://img.shields.io/badge/C++-17-blue.svg?style=flat&logo=c%2B%2B
+[c++standard]: https://isocpp.org/std/the-standard [Nightly-Build]: https://
+github.com/KratosMultiphysics/Kratos/workflows/Nightly%20Build/badge.svg
+[Nightly-link]: https://github.com/KratosMultiphysics/Kratos/
+actions?query=workflow%3A%22Nightly+Build%22 [DOI-image]: https://zenodo.org/
+badge/DOI/10.5281/zenodo.3234644.svg [DOI]: https://doi.org/10.5281/
+zenodo.3234644 [stars-image]: https://img.shields.io/github/stars/
+KratosMultiphysics/Kratos?label=Stars&logo=github [stars]: https://github.com/
+KratosMultiphysics/Kratos/stargazers [twitter-image]: https://img.shields.io/
+twitter/follow/kratosmultiphys.svg?label=Follow&style=social [twitter]: https:/
+/twitter.com/kratosmultiphys [youtube-image]: https://badges.aleen42.com/src/
+youtube.svg [youtube]:https://www.youtube.com/@kratosmultiphysics3578 _KRATOS
+Multiphysics_ ("Kratos") is a framework for building parallel, multi-
+disciplinary simulation software, aiming at modularity, extensibility, and high
+performance. Kratos is written in C++, and counts with an extensive Python
+interface. More in [Overview](https://github.com/KratosMultiphysics/Kratos/
+wiki/Overview) **Kratos** is **free** under BSD-4 [license](https://github.com/
+KratosMultiphysics/Kratos/wiki/Licence) and can be used even in comercial
+softwares as it is. Many of its main applications are also free and BSD-
+4 licensed but each derived application can have its own propietary license. #
+Main Features **Kratos** is __multiplatform__ and available for __Windows,
+Linux__ (several distros) and __macOS__. **Kratos** is __OpenMP__ and __MPI__
+parallel and scalable up to thousands of cores. **Kratos** provides a core
+which defines the common framework and several application which work like
+plug-ins that can be extended in diverse fields. ## Its main applications are:
+- [DEM](applications/DEMApplication) for cohesive and non cohesive spheric and
+non spheric particles simulation - [Fluid Dynamics](applications/
+FluidDynamicsApplication/README.md) Provides 2D and 3D incompressible fluids
+formulation - [Fluid Structure Interaction](applications/FSIApplication/
+README.md) for solution of different FSI problems - [Structural Mechanics]
+(applications/StructuralMechanicsApplication/README.md) Providing solution for
+solid, shell and beam structures with linear and nonlinear, static and dynamic
+behavior - [Contact Structural Mechanics](applications/
 ContactStructuralMechanicsApplication/README.md) For contact problems used
 along the [Structural Mechanics application](applications/
 StructuralMechanicsApplication/README.md) ## Some main modules are: - [Linear
 Solvers](applications/LinearSolversApplication/README.md) - [Trilinos]
 (applications/TrilinosApplication/README.md) - [Metis](applications/
 MetisApplication/README.md) - [Meshing](applications/MeshingApplication/
 README.md) # Documentation Here you can find the basic documentation of the
```

