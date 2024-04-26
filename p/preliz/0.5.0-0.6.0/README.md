# Comparing `tmp/preliz-0.5.0.tar.gz` & `tmp/preliz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.5.0.tar` & `preliz-0.6.0.tar`

### file list

```diff
@@ -1,83 +1,102 @@
--rw-r--r--   0        0        0     4324 2024-04-12 12:55:33.124757 preliz-0.5.0/README.md
--rw-r--r--   0        0        0      649 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/__init__.py
--rw-r--r--   0        0        0     1154 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/__init__.py
--rw-r--r--   0        0        0     6930 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/asymmetric_laplace.py
--rw-r--r--   0        0        0     5012 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/bernoulli.py
--rw-r--r--   0        0        0     7701 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/beta.py
--rw-r--r--   0        0        0     5242 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/binomial.py
--rw-r--r--   0        0        0     4723 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/categorical.py
--rw-r--r--   0        0        0     7476 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/censored.py
--rw-r--r--   0        0        0    42469 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/continuous.py
--rw-r--r--   0        0        0    21548 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0    10600 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/discrete.py
--rw-r--r--   0        0        0     5071 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/discrete_uniform.py
--rw-r--r--   0        0        0    26023 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0     4391 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/exponential.py
--rw-r--r--   0        0        0     5866 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/gamma.py
--rw-r--r--   0        0        0     3885 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/geometric.py
--rw-r--r--   0        0        0     4920 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/halfnormal.py
--rw-r--r--   0        0        0     7938 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/halfstudentt.py
--rw-r--r--   0        0        0     6452 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/inversegamma.py
--rw-r--r--   0        0        0     4061 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/laplace.py
--rw-r--r--   0        0        0     6033 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/negativebinomial.py
--rw-r--r--   0        0        0     5092 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/normal.py
--rw-r--r--   0        0        0     4194 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/poisson.py
--rw-r--r--   0        0        0     7610 2024-04-12 12:55:33.180757 preliz-0.5.0/preliz/distributions/studentt.py
--rw-r--r--   0        0        0     6875 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/triangular.py
--rw-r--r--   0        0        0     5668 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/truncated.py
--rw-r--r--   0        0        0     4692 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/uniform.py
--rw-r--r--   0        0        0     4987 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/vonmises.py
--rw-r--r--   0        0        0     5763 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/wald.py
--rw-r--r--   0        0        0     5068 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/weibull.py
--rw-r--r--   0        0        0     5562 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/zi_binomial.py
--rw-r--r--   0        0        0     7223 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/zi_negativebinomial.py
--rw-r--r--   0        0        0     5667 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/distributions/zi_poisson.py
--rw-r--r--   0        0        0       64 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4540 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0    13847 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/optimization.py
--rw-r--r--   0        0        0     5596 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/parser.py
--rw-r--r--   0        0        0    19567 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     9785 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0     2028 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/predictive_helper.py
--rw-r--r--   0        0        0    11407 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/internal/special.py
--rw-r--r--   0        0        0     6465 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/ppls/pymc_io.py
--rw-r--r--   0        0        0      145 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14617 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     2251 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/ppe.py
--rw-r--r--   0        0        0     2160 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/predictive/predictive_explorer.py
--rw-r--r--   0        0        0     1946 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1787 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0   477854 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/ppa.ipynb
--rw-r--r--   0        0        0     2787 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/predictive_explorer.ipynb
--rw-r--r--   0        0        0     1439 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/quartile_int.ipynb
--rw-r--r--   0        0        0     1472 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0      661 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_beta_mode.py
--rw-r--r--   0        0        0     1967 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_censored.py
--rw-r--r--   0        0        0      757 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_dirichlet_mode.py
--rw-r--r--   0        0        0     7196 2024-04-12 12:55:33.184757 preliz-0.5.0/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      346 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_distributions_helper.py
--rw-r--r--   0        0        0      626 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_helper.py
--rw-r--r--   0        0        0      338 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6659 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2919 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_mle.py
--rw-r--r--   0        0        0      894 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_optimization.py
--rw-r--r--   0        0        0     5964 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_plots.py
--rw-r--r--   0        0        0       85 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_ppa.py
--rw-r--r--   0        0        0      117 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_predictive_explorer.py
--rw-r--r--   0        0        0     3489 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      103 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_quartile_int.py
--rw-r--r--   0        0        0      910 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0     7665 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_scipy.py
--rw-r--r--   0        0        0     1595 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_special.py
--rw-r--r--   0        0        0     2589 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/tests/test_truncated.py
--rw-r--r--   0        0        0      325 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/beta_mode.py
--rw-r--r--   0        0        0     2341 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/dirichlet_mode.py
--rw-r--r--   0        0        0     4125 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1654 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3259 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     6136 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/quartile_int.py
--rw-r--r--   0        0        0    12994 2024-04-12 12:55:33.188757 preliz-0.5.0/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1410 2024-04-12 12:55:33.188757 preliz-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5568 1970-01-01 00:00:00.000000 preliz-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4324 2024-04-26 20:09:30.590731 preliz-0.6.0/README.md
+-rw-r--r--   0        0        0      649 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/__init__.py
+-rw-r--r--   0        0        0     2772 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0     6930 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/asymmetric_laplace.py
+-rw-r--r--   0        0        0     5012 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/bernoulli.py
+-rw-r--r--   0        0        0     7701 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/beta.py
+-rw-r--r--   0        0        0     6721 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/betabinomial.py
+-rw-r--r--   0        0        0     7062 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/betascaled.py
+-rw-r--r--   0        0        0     5242 2024-04-26 20:09:30.646732 preliz-0.6.0/preliz/distributions/binomial.py
+-rw-r--r--   0        0        0     4723 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/categorical.py
+-rw-r--r--   0        0        0     4302 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/cauchy.py
+-rw-r--r--   0        0        0     7488 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/censored.py
+-rw-r--r--   0        0        0     4233 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/chi_squared.py
+-rw-r--r--   0        0        0    21635 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0     5071 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/discrete_uniform.py
+-rw-r--r--   0        0        0     4942 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/discrete_weibull.py
+-rw-r--r--   0        0        0    25352 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0     5946 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/exgaussian.py
+-rw-r--r--   0        0        0     4391 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/exponential.py
+-rw-r--r--   0        0        0     5866 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/gamma.py
+-rw-r--r--   0        0        0     3885 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/geometric.py
+-rw-r--r--   0        0        0     4489 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/gumbel.py
+-rw-r--r--   0        0        0     3920 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/halfcauchy.py
+-rw-r--r--   0        0        0     4920 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/halfnormal.py
+-rw-r--r--   0        0        0     7938 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/halfstudentt.py
+-rw-r--r--   0        0        0     5386 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/hurdle.py
+-rw-r--r--   0        0        0     6141 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/hypergeometric.py
+-rw-r--r--   0        0        0     6452 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/inversegamma.py
+-rw-r--r--   0        0        0     4798 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/kumaraswamy.py
+-rw-r--r--   0        0        0     4061 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/laplace.py
+-rw-r--r--   0        0        0     3862 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/logistic.py
+-rw-r--r--   0        0        0     5742 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/logitnormal.py
+-rw-r--r--   0        0        0     5013 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/lognormal.py
+-rw-r--r--   0        0        0     4710 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/moyal.py
+-rw-r--r--   0        0        0     6033 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/negativebinomial.py
+-rw-r--r--   0        0        0     5017 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/normal.py
+-rw-r--r--   0        0        0     5067 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/pareto.py
+-rw-r--r--   0        0        0     4194 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/poisson.py
+-rw-r--r--   0        0        0     5851 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/rice.py
+-rw-r--r--   0        0        0     6212 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/skewnormal.py
+-rw-r--r--   0        0        0     7610 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/studentt.py
+-rw-r--r--   0        0        0     6875 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/triangular.py
+-rw-r--r--   0        0        0     5680 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/truncated.py
+-rw-r--r--   0        0        0    14611 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/truncatednormal.py
+-rw-r--r--   0        0        0     4692 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/uniform.py
+-rw-r--r--   0        0        0     4987 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/vonmises.py
+-rw-r--r--   0        0        0     5665 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/wald.py
+-rw-r--r--   0        0        0     5068 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/weibull.py
+-rw-r--r--   0        0        0     5560 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/zi_binomial.py
+-rw-r--r--   0        0        0     7223 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/zi_negativebinomial.py
+-rw-r--r--   0        0        0     5667 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/distributions/zi_poisson.py
+-rw-r--r--   0        0        0       64 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4540 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0    13819 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     5596 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/parser.py
+-rw-r--r--   0        0        0    19087 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     9785 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0     2028 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/predictive_helper.py
+-rw-r--r--   0        0        0    11863 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/internal/special.py
+-rw-r--r--   0        0        0     6465 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/ppls/pymc_io.py
+-rw-r--r--   0        0        0      145 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14606 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     2251 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/ppe.py
+-rw-r--r--   0        0        0     2160 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/predictive/predictive_explorer.py
+-rw-r--r--   0        0        0     1946 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1787 2024-04-26 20:09:30.650732 preliz-0.6.0/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0   477854 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/ppa.ipynb
+-rw-r--r--   0        0        0     2787 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/predictive_explorer.ipynb
+-rw-r--r--   0        0        0     1439 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/quartile_int.ipynb
+-rw-r--r--   0        0        0     1472 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0      661 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_beta_mode.py
+-rw-r--r--   0        0        0     1967 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_censored.py
+-rw-r--r--   0        0        0      757 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_dirichlet_mode.py
+-rw-r--r--   0        0        0     1144 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_discrete_weibull.py
+-rw-r--r--   0        0        0     7265 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      346 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_distributions_helper.py
+-rw-r--r--   0        0        0      626 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0     2292 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_hurdle.py
+-rw-r--r--   0        0        0      338 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6654 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2919 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0      987 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_optimization.py
+-rw-r--r--   0        0        0     6153 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0       85 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_ppa.py
+-rw-r--r--   0        0        0      117 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_predictive_explorer.py
+-rw-r--r--   0        0        0     3475 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      103 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_quartile_int.py
+-rw-r--r--   0        0        0      910 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0    10795 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_scipy.py
+-rw-r--r--   0        0        0     1851 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_special.py
+-rw-r--r--   0        0        0     2568 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/tests/test_truncated.py
+-rw-r--r--   0        0        0      325 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/beta_mode.py
+-rw-r--r--   0        0        0     2341 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/dirichlet_mode.py
+-rw-r--r--   0        0        0     4125 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1654 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3259 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     6136 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/quartile_int.py
+-rw-r--r--   0        0        0    12994 2024-04-26 20:09:30.654732 preliz-0.6.0/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1410 2024-04-26 20:09:30.654732 preliz-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5568 1970-01-01 00:00:00.000000 preliz-0.6.0/PKG-INFO
```

### Comparing `preliz-0.5.0/README.md` & `preliz-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/__init__.py` & `preliz-0.6.0/preliz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.5.0/preliz/distributions/asymmetric_laplace.py` & `preliz-0.6.0/preliz/distributions/asymmetric_laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/bernoulli.py` & `preliz-0.6.0/preliz/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/beta.py` & `preliz-0.6.0/preliz/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/binomial.py` & `preliz-0.6.0/preliz/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/categorical.py` & `preliz-0.6.0/preliz/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/censored.py` & `preliz-0.6.0/preliz/distributions/censored.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pylint: disable=arguments-differ
 import numpy as np
 
-from preliz.distributions.distributions import TruncatedCensored
+from preliz.distributions.distributions import DistributionTransformer
 from preliz.internal.distribution_helper import all_not_none
 from preliz.internal.special import xlogx, xprody
 from preliz.distributions.truncated import Truncated
 
 
-class Censored(TruncatedCensored):
+class Censored(DistributionTransformer):
     r"""
     Censored distribution
 
     This is not a distribution per se, but a modifier of univariate distributions.
 
     Given a base distribution with cumulative distribution function (CDF) and
     probability density mass/function (PDF). The pdf of a Censored distribution is:
```

### Comparing `preliz-0.5.0/preliz/distributions/continuous_multivariate.py` & `preliz-0.6.0/preliz/distributions/continuous_multivariate.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 
 try:
     from ipywidgets import interactive, widgets
 except ImportError:
     pass
 from scipy import stats
 
+from .beta import Beta  # pylint: disable=no-name-in-module
+from .normal import Normal  # pylint: disable=no-name-in-module
 from .distributions_multivariate import Continuous
-from .continuous import Beta, Normal
 from ..internal.distribution_helper import all_not_none
 from ..internal.plot_helper_multivariate import plot_dirichlet, plot_mvnormal
 from ..internal.plot_helper import check_inside_notebook, get_slider
 
 eps = np.finfo(float).eps
```

### Comparing `preliz-0.5.0/preliz/distributions/discrete_uniform.py` & `preliz-0.6.0/preliz/distributions/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/distributions.py` & `preliz-0.6.0/preliz/distributions/distributions.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,43 +30,32 @@
     """
     Base class for distributions.
 
     Not intended for direct instantiation.
     """
 
     def __init__(self):
-        self.rv_frozen = None
         self.is_frozen = False
         self.opt = None
 
     def __repr__(self):
         name = self.__class__.__name__
-        if name == "Truncated":
-            name += self.dist.__class__.__name__
-        elif name == "Censored":
+        if name in ["Truncated", "Censored", "Hurdle"]:
             name += self.dist.__class__.__name__
         if self.is_frozen:
             bolded_name = "\033[1m" + name + "\033[0m"
 
             description = "".join(
                 f"{n}={np.round(v, 2)}," for n, v in zip(self.param_names, self.params)
             ).strip(",")
 
             return f"{bolded_name}({description})"
         else:
             return name
 
-    def _update_rv_frozen(self):
-        """Update the rv_frozen object"""
-
-        frozen = self._get_frozen()
-        if frozen is not None:
-            self.is_frozen = True
-            self.rv_frozen = frozen
-
     def summary(self, mass=0.94, fmt=".2f"):
         """
         Namedtuple with the mean, median, standard deviation, and lower and upper bounds
         of the equal-tailed interval.
 
         Parameters
         ----------
@@ -104,51 +93,51 @@
         Parameters
         ----------
         size : int or tuple of ints, optional
             Defining number of random variates. Defaults to 1.
         random_state : {None, int, numpy.random.Generator, numpy.random.RandomState}
             Defaults to None
         """
-        return self.rv_frozen.rvs(*args, **kwds)
+        return self.rvs(*args, **kwds)
 
     def cdf(self, x, *args, **kwds):
         """Cumulative distribution function.
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the cdf
         """
-        return self.rv_frozen.cdf(x, *args, **kwds)
+        return self.cdf(x, *args, **kwds)
 
     def ppf(self, q, *args, **kwds):
         """Percent point function (inverse of cdf).
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the inverse of the cdf
         """
-        return self.rv_frozen.ppf(q, *args, **kwds)
+        return self.ppf(q, *args, **kwds)
 
     def mean(self):
         """Mean of the distribution."""
-        return self.rv_frozen.mean()
+        return self.mean()
 
     def median(self):
         """Median of the distribution."""
-        return self.rv_frozen.median()
+        return self.median()
 
     def std(self):
         """Standard deviation of the distribution."""
-        return self.rv_frozen.std()
+        return self.std()
 
     def var(self):
         """Variance of the distribution."""
-        return self.rv_frozen.var()
+        return self.var()
 
     def skewness(self):
         """Skewness of the distribution."""
         return self.stats(moment="s")
 
     def kurtosis(self):
         """Kurtosis of the distribution"""
@@ -163,34 +152,31 @@
         Parameters
         ----------
         types : str
             The type of moments to compute. Default is 'mvsk'
             where 'm' = mean, 'v' = variance, 's' = skewness, and 'k' = kurtosis.
             Valid combinations are any subset of 'mvsk'.
         """
-        if self.rv_frozen is None:
-            moments = []
-            for m_t in types:
-                if m_t not in "mdvsk":
-                    raise ValueError(
-                        "The input string should only contain the letters "
-                        "'m', 'd', 'v', 's', or 'k'."
-                    )
-                if m_t == "m":
-                    moments.append(self.mean())
-                elif m_t == "d":
-                    moments.append(self.std())
-                elif m_t == "v":
-                    moments.append(self.var())
-                elif m_t == "s":
-                    moments.append(self.skewness())
-                elif m_t == "k":
-                    moments.append(self.kurtosis())
-        else:
-            moments = self.rv_frozen.stats(moments=types)
+        moments = []
+        for m_t in types:
+            if m_t not in "mdvsk":
+                raise ValueError(
+                    "The input string should only contain the letters "
+                    "'m', 'd', 'v', 's', or 'k'."
+                )
+            if m_t == "m":
+                moments.append(self.mean())
+            elif m_t == "d":
+                moments.append(self.std())
+            elif m_t == "v":
+                moments.append(self.var())
+            elif m_t == "s":
+                moments.append(self.skewness())
+            elif m_t == "k":
+                moments.append(self.kurtosis())
 
         return moments
 
     def eti(self, mass=0.94, fmt=".2f"):
         """Equal-tailed interval containing `mass`.
 
         Parameters
@@ -203,18 +189,15 @@
         """
         valid_distribution(self)
 
         if not isinstance(fmt, str):
             raise ValueError("Invalid format string.")
 
         if valid_scalar_params(self):
-            if self.rv_frozen is None:
-                eti_b = self.ppf([(1 - mass) / 2, 1 - (1 - mass) / 2])
-            else:
-                eti_b = self.rv_frozen.interval(mass)
+            eti_b = self.ppf([(1 - mass) / 2, 1 - (1 - mass) / 2])
             lower_tail = float(f"{eti_b[0]:{fmt}}")
             upper_tail = float(f"{eti_b[1]:{fmt}}")
             return (lower_tail, upper_tail)
         else:
             return None
 
     def hdi(self, mass=0.94, fmt=".2f"):
@@ -638,25 +621,25 @@
         """Probability density function at x.
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the pdf
         """
-        return self.rv_frozen.pdf(x, *args, **kwds)
+        return self.pdf(x, *args, **kwds)
 
     def logpdf(self, x, *args, **kwds):
         """Probability mass function at x.
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the pdf
         """
-        return self.rv_frozen.logpdf(x, *args, **kwds)
+        return self.logpdf(x, *args, **kwds)
 
 
 class Discrete(Distribution):
     """Base class for discrete distributions."""
 
     def __init__(self):
         super().__init__()
@@ -684,29 +667,29 @@
         """Probability mass function at x.
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the pdf
         """
-        return self.rv_frozen.pmf(x, *args, **kwds)
+        return self.pdf(x, *args, **kwds)
 
     def logpdf(self, x, *args, **kwds):
         """Probability mass function at x.
 
         Parameters
         ----------
         x : array_like
             Values on which to evaluate the pdf
         """
-        return self.rv_frozen.logpmf(x, *args, **kwds)
+        return self.logpdf(x, *args, **kwds)
 
 
-class TruncatedCensored(Distribution):
-    """Base class for discrete distributions."""
+class DistributionTransformer(Distribution):
+    """Base class for distributions that transform other distributions"""
 
     def __init__(self):
         super().__init__()
         self.kind = self.dist.kind
 
     def xvals(self, support, n_points=None):
         """Provide x values in the support of the distribution. This is useful for example when
```

### Comparing `preliz-0.5.0/preliz/distributions/distributions_multivariate.py` & `preliz-0.6.0/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/exponential.py` & `preliz-0.6.0/preliz/distributions/exponential.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/gamma.py` & `preliz-0.6.0/preliz/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/geometric.py` & `preliz-0.6.0/preliz/distributions/geometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/halfnormal.py` & `preliz-0.6.0/preliz/distributions/halfnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/halfstudentt.py` & `preliz-0.6.0/preliz/distributions/halfstudentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/inversegamma.py` & `preliz-0.6.0/preliz/distributions/inversegamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/laplace.py` & `preliz-0.6.0/preliz/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/negativebinomial.py` & `preliz-0.6.0/preliz/distributions/negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/normal.py` & `preliz-0.6.0/preliz/distributions/normal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=arguments-differ
 import numba as nb
 import numpy as np
-from scipy.special import erf, erfinv  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, to_precision, from_precision, all_not_none
 from ..internal.special import erf, erfinv, mean_and_std, ppf_bounds_cont
 
 
 class Normal(Continuous):
```

### Comparing `preliz-0.5.0/preliz/distributions/poisson.py` & `preliz-0.6.0/preliz/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/studentt.py` & `preliz-0.6.0/preliz/distributions/studentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/triangular.py` & `preliz-0.6.0/preliz/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/truncated.py` & `preliz-0.6.0/preliz/distributions/truncated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=arguments-differ
 import numpy as np
 
-from preliz.distributions.distributions import TruncatedCensored
+from preliz.distributions.distributions import DistributionTransformer
 from preliz.internal.distribution_helper import all_not_none
 
 
-class Truncated(TruncatedCensored):
+class Truncated(DistributionTransformer):
     r"""
     Truncated distribution
 
     This is not a distribution per se, but a modifier of univariate distributions.
 
     Given a base distribution with cumulative distribution function (CDF) and
     probability density mass/function (PDF). The pdf of a Truncated distribution is:
```

### Comparing `preliz-0.5.0/preliz/distributions/uniform.py` & `preliz-0.6.0/preliz/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/vonmises.py` & `preliz-0.6.0/preliz/distributions/vonmises.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/wald.py` & `preliz-0.6.0/preliz/distributions/wald.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # pylint: disable=invalid-name
 import numba as nb
 import numpy as np
 from scipy.special import ndtr, expi  # pylint: disable=no-name-in-module
 
 from .distributions import Continuous
 from ..internal.distribution_helper import eps, all_not_none
-from ..internal.special import cdf_bounds, ppf_bounds_cont
+from ..internal.special import cdf_bounds
 from ..internal.optimization import optimize_ml, find_ppf
 
 
 class Wald(Continuous):
     r"""
     Wald distribution.
 
@@ -131,15 +131,15 @@
         return nb_cdf(x, self.mu, self.lam)
 
     def ppf(self, q):
         """
         Compute the percent point function (PPF) at a given probability q.
         """
         q = np.asarray(q)
-        return nb_ppf(q, self)
+        return find_ppf(self, q)
 
     def logpdf(self, x):
         """
         Compute the log probability density function (log PDF) at a given point x.
         """
         return nb_logpdf(x, self.mu, self.lam)
 
@@ -186,18 +186,14 @@
     x = np.asarray(x)
     u = (lam / (x + eps)) ** 0.5
     v = x / mu
     z = ndtr(u * (v - 1)) + np.exp(2 * lam / mu) * ndtr(-u * (v + 1))
     return cdf_bounds(z, x, 0, np.inf)
 
 
-def nb_ppf(q, dist):
-    return ppf_bounds_cont(find_ppf(dist, q), q, 0, np.inf)
-
-
 def nb_entropy(mu, lam):
     return 0.5 * np.log((2 * np.pi * np.e * mu**3) / lam) + 3 / 2 * np.exp(2 * lam / mu) * expi(
         -2 * lam / mu
     )
 
 
 @nb.vectorize(nopython=True, cache=True)
```

### Comparing `preliz-0.5.0/preliz/distributions/weibull.py` & `preliz-0.6.0/preliz/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/zi_binomial.py` & `preliz-0.6.0/preliz/distributions/zi_binomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             \end{array} \right.
 
     .. plot::
         :context: close-figs
 
         import arviz as az
         from preliz import ZeroInflatedBinomial
-        az.style.use('arviz-white')
+        az.style.use('arviz-doc')
         ns = [10, 20]
         ps = [0.5, 0.7]
         psis = [0.7, 0.4]
         for n, p, psi in zip(ns, ps, psis):
             ZeroInflatedBinomial(psi, n, p).plot_pdf(support=(0,25))
 
     ========  ==========================
```

### Comparing `preliz-0.5.0/preliz/distributions/zi_negativebinomial.py` & `preliz-0.6.0/preliz/distributions/zi_negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/distributions/zi_poisson.py` & `preliz-0.6.0/preliz/distributions/zi_poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/internal/distribution_helper.py` & `preliz-0.6.0/preliz/internal/distribution_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/internal/optimization.py` & `preliz-0.6.0/preliz/internal/optimization.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Optimization routines and utilities
 """
 from sys import modules
 import warnings
 from copy import copy
 
 import numpy as np
-from scipy.optimize import minimize, least_squares, root_scalar
+from scipy.optimize import minimize, least_squares, root_scalar, brentq
 from scipy.special import i0, i1, i0e, i1e  # pylint: disable=no-name-in-module
 from .distribution_helper import init_vals as default_vals
 
 
 def optimize_max_ent(dist, lower, upper, mass, none_idx, fixed):
     def prob_bound(params, dist, lower, upper, mass):
         params = get_params(dist, params, none_idx, fixed)
@@ -21,18 +21,15 @@
         cdf1 = dist.cdf(upper)
         loss = (cdf1 - cdf0) - mass
         return loss
 
     def entropy_loss(params, dist):
         params = get_params(dist, params, none_idx, fixed)
         dist._parametrization(**params)
-        if dist.rv_frozen is None:
-            return -dist.entropy()
-        else:
-            return -dist.rv_frozen.entropy()
+        return -dist.entropy()
 
     cons = {
         "type": "eq",
         "fun": prob_bound,
         "args": (dist, lower, upper, mass),
     }
     init_vals = np.array(dist.params)[none_idx]
@@ -175,15 +172,15 @@
 
     return nu, sigma
 
 
 def optimize_ml(dist, sample):
     def negll(params, dist, sample):
         dist._update(*params)
-        return -dist.logpdf(sample).sum()
+        return dist._neg_logpdf(sample)
 
     dist._fit_moments(np.mean(sample), np.std(sample))
     init_vals = dist.params
 
     opt = minimize(negll, x0=init_vals, bounds=dist.params_support, args=(dist, sample))
 
     dist._update(*opt["x"])
@@ -311,15 +308,15 @@
         if dist.__class__.__name__ in ["BetaScaled", "TruncatedNormal"]:
             update_bounds_beta_scaled(dist, x_min, x_max)
 
         loss = np.inf
         if dist._check_endpoints(x_min, x_max, raise_error=False):
             dist._fit_mle(sample)  # pylint:disable=protected-access
             corr = get_penalization(sample_size, dist)
-            loss = -(dist.logpdf(sample).sum() - corr)
+            loss = dist._neg_logpdf(sample) + corr
 
         fitted.update(loss, dist)
 
     return fitted
 
 
 def fit_to_quartile(dist_names, q1, q2, q3, extra_pros):
@@ -412,43 +409,46 @@
         )
         return root_res.root
     else:
         return np.finfo(float).tiny
 
 
 def find_ppf(dist, q):
-    """
-    Function to find the percent point function (ppf) given the
-    cumulative distribution function (cdf).
-
-    Parameters
-    ----------
-
-    dist : preliz distribution
-        The distribution for which to find the ppf.
-    q : float or list-like
-        The required quantile(s) for which to find the ppf.
-    """
-
-    def objective(x, dist, q):
-        return np.sum((dist.cdf(x) - q) ** 2)
-
-    q = np.asarray(q)
-    initial_guess, bounds = initialize_ppf(dist, q)
-    opt = minimize(objective, x0=initial_guess, method="Powell", bounds=bounds, args=(dist, q))
+    q = np.atleast_1d(q)
+    ppf = np.zeros_like(q)
+    lower, upper = dist.support
+    for idx, q_i in enumerate(q):
+        if q_i < 0:
+            ppf[idx] = np.nan
+        elif q_i > 1:
+            ppf[idx] = np.nan
+        elif q_i == 0:
+            if dist.kind == "discrete":
+                ppf[idx] = lower - 1
+            else:
+                ppf[idx] = lower
+        elif q_i == 1:
+            ppf[idx] = upper
+        else:
+            if dist.__class__.__name__ in ["HyperGeometric", "BetaBinomial"]:
+                ppf[idx] = _ppf_single(dist, q_i) + 1
+            else:
+                ppf[idx] = _ppf_single(dist, q_i)
+    return ppf[0] if len(ppf) == 1 else ppf
 
-    return opt["x"]
 
+def _ppf_single(dist, q):
+    def func(x, dist, q):
+        return dist.cdf(x) - q
 
-def initialize_ppf(dist, q):
-    # Calculate k using the formula for Chebyshev's inequality
-    q = np.clip(q, 0.1, 0.9)
-    k = np.sqrt(1 / (1 - q))
+    factor = 10.0
+    left, right = dist.support
 
-    k = np.where(q < 0.5, -k, k)
+    left = min(-factor, right)
+    while func(left, dist, q) > 0.0:
+        left, right = left * factor, left
 
-    initial_guess = dist.mean() + k * dist.std()
-    lower, upper = dist.support
-    np.where(initial_guess < lower, lower, np.where(initial_guess > upper, upper, initial_guess))
-    bounds = [(lower, upper)]
+    right = max(factor, left)
+    while func(right, dist, q) < 0.0:
+        left, right = right, right * factor
 
-    return initial_guess, bounds
+    return brentq(func, left, right, args=(dist, q))
```

### Comparing `preliz-0.5.0/preliz/internal/parser.py` & `preliz-0.6.0/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/internal/plot_helper.py` & `preliz-0.6.0/preliz/internal/plot_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import inspect
-import logging
 import traceback
 import sys
 
-
 try:
     from IPython import get_ipython
     from ipywidgets import FloatSlider, IntSlider, FloatText, IntText, Checkbox, ToggleButton
 except ImportError:
     pass
 
 from arviz import plot_kde, plot_ecdf, hdi
 from arviz.stats.density_utils import _kde_linear
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import _pylab_helpers, get_backend
 from matplotlib.ticker import MaxNLocator
-from scipy.interpolate import interp1d, PchipInterpolator
-
-_log = logging.getLogger("preliz")
 
 
 def plot_pointinterval(distribution, interval="hdi", levels=None, rotated=False, ax=None):
     """
     Plot median as a dot and intervals as lines.
     By defaults the intervals are HDI with 0.5 and 0.94 mass.
 
@@ -148,26 +143,16 @@
         mass = dist.pdf(x)
 
         if dist.__class__.__name__ in ["Categorical", "Bernoulli"]:
             p = ax.plot(x, mass, "o", label=label, color=color, alpha=alpha)
             ax.vlines(x, 0, mass, ls="dotted", color=p[0].get_color(), alpha=alpha)
         else:
             x_c = np.linspace(x[0], x[-1], 1000)
-            # if new distribution, directly compute pdf at non-integer values
-            print(dist.__class__.__name__)
-            if dist.rv_frozen is None:
-                mass_c = np.clip(dist.pdf(x_c), np.min(mass), np.max(mass))
-            # if old, interpolate
-            else:
-                if len(x) > 2:
-                    interp = PchipInterpolator(x, mass)
-                else:
-                    interp = interp1d(x, mass)
-
-                mass_c = np.clip(interp(x_c), np.min(mass), np.max(mass))
+            # we compute pmf at non-integer values to get a continuous curve
+            mass_c = np.clip(dist.pdf(x_c), np.min(mass), np.max(mass))
 
             p = ax.plot(x_c, mass_c, ls="dotted", color=color, alpha=alpha)
             ax.plot(x, mass, "o", label=label, color=p[0].get_color(), alpha=alpha)
 
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
         ax.axhline(0, color="0.8", ls="--", zorder=0)
```

### Comparing `preliz-0.5.0/preliz/internal/plot_helper_multivariate.py` & `preliz-0.6.0/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/internal/predictive_helper.py` & `preliz-0.6.0/preliz/internal/predictive_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/internal/special.py` & `preliz-0.6.0/preliz/internal/special.py`

 * *Files 11% similar despite different names*

```diff
@@ -113,14 +113,19 @@
 
 
 @nb.njit(cache=True)
 def erfinv(p):
     return -erfcinv(p + 1)
 
 
+@nb.njit(cache=True)
+def erfcx(x):
+    return np.exp(x**2) * erfc(x)
+
+
 @nb.vectorize(nopython=True, cache=True)
 def beta(a, b):
     if a < 0 or b < 0:
         raise ValueError("Arguments must be positive.")
     elif a == 0 and b == 0:
         return np.inf
     elif a == 0 or b == 0:
@@ -430,14 +435,34 @@
     for j in range(6):
         x = x + 1
         ser = ser + cof[j] / x
     return tmp + np.log(stp * ser)
 
 
 @nb.vectorize(nopython=True, cache=True)
+def logit(x):
+    if x == 0:
+        return -np.inf
+    elif x == 1:
+        return np.inf
+    if x < 0 or x > 1:
+        return np.nan
+    else:
+        return np.log(x / (1 - x))
+
+
+@nb.vectorize(nopython=True, cache=True)
+def expit(x):
+    if x >= 0:
+        return 1 / (1 + np.exp(-x))
+    else:
+        return np.exp(x) / (1 + np.exp(x))
+
+
+@nb.vectorize(nopython=True, cache=True)
 def xlogy(x, y):
     if x == 0:
         return 0.0
     else:
         return x * np.log(y)
```

### Comparing `preliz-0.5.0/preliz/ppls/pymc_io.py` & `preliz-0.6.0/preliz/ppls/pymc_io.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/predictive/ppa.py` & `preliz-0.6.0/preliz/predictive/ppa.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ..internal.plot_helper import (
     check_inside_notebook,
     plot_pp_samples,
     plot_pp_mean,
 )
 from ..internal.parser import get_prior_pp_samples, from_preliz, from_bambi
 from ..internal.predictive_helper import back_fitting, select_prior_samples
-from ..distributions.continuous import Normal
+from ..distributions import Normal
 from ..distributions.distributions import Distribution
 
 _log = logging.getLogger("preliz")
 
 
 def ppa(
     fmodel, draws=2000, references=0, boundaries=(-np.inf, np.inf), target=None, engine="preliz"
```

### Comparing `preliz-0.5.0/preliz/predictive/ppe.py` & `preliz-0.6.0/preliz/predictive/ppe.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/predictive/predictive_explorer.py` & `preliz-0.6.0/preliz/predictive/predictive_explorer.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.6.0/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/plot_interactive.ipynb` & `preliz-0.6.0/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/ppa.ipynb` & `preliz-0.6.0/preliz/tests/ppa.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/predictive_explorer.ipynb` & `preliz-0.6.0/preliz/tests/predictive_explorer.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/quartile_int.ipynb` & `preliz-0.6.0/preliz/tests/quartile_int.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/roulette.ipynb` & `preliz-0.6.0/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_beta_mode.py` & `preliz-0.6.0/preliz/tests/test_beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_censored.py` & `preliz-0.6.0/preliz/tests/test_censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_dirichlet_mode.py` & `preliz-0.6.0/preliz/tests/test_dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_distributions.py` & `preliz-0.6.0/preliz/tests/test_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from numpy.testing import assert_almost_equal
 import numpy as np
 from test_helper import run_notebook
 
 from preliz.distributions import (
     AsymmetricLaplace,
     Beta,
+    BetaScaled,
     Cauchy,
     ChiSquared,
     Gamma,
     Gumbel,
     ExGaussian,
     Exponential,
     HalfCauchy,
@@ -133,14 +134,15 @@
 
 
 @pytest.mark.parametrize(
     "distribution, params",
     [
         (AsymmetricLaplace, (1, 4, 3)),
         (Beta, (2, 5)),
+        (BetaScaled, (2, 2, -1, 2)),
         (Cauchy, (0, 1)),
         (ChiSquared, (1,)),
         (ExGaussian, (0, 1, 3)),
         (Exponential, (0.5,)),
         (Gamma, (1, 0.5)),
         (Gumbel, (0, 1)),
         (HalfCauchy, (1,)),
@@ -187,15 +189,15 @@
 )
 def test_mle(distribution, params):
     dist = distribution(*params)
     sample = dist.rvs(20000)
     dist_ = distribution()
     dist_._fit_mle(sample)
 
-    if dist.__class__.__name__ == "Pareto":
+    if dist.__class__.__name__ in ["Pareto", "ExGaussian"]:
         tol = 0
     else:
         tol = 1
     assert_almost_equal(dist.mean(), dist_.mean(), tol)
     assert_almost_equal(dist.std(), dist_.std(), tol)
     if dist.__class__.__name__ == "StudentT":
         assert_almost_equal(params[1:], dist_.params[1:], 0)
```

### Comparing `preliz-0.5.0/preliz/tests/test_helper.py` & `preliz-0.6.0/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_maxent.py` & `preliz-0.6.0/preliz/tests/test_maxent.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,46 +71,46 @@
             (-0.799, 0.260),
         ),
         (Beta(), 0.2, 0.6, 0.9, (0, 1), (6.112, 9.101)),
         (BetaScaled(lower=-2, upper=3), -1, 1, 0.8, (-2, 3), (3.883, 5.560)),
         (Cauchy(), -1, 1, 0.6, (-np.inf, np.inf), (0, 0.726)),
         (Cauchy(alpha=0.5), -1, 1, 0.6, (-np.inf, np.inf), (0.6000)),
         (ChiSquared(), 2, 7, 0.6, (0, np.inf), (4.002)),
-        (ExGaussian(), 9, 10, 0.8, (-np.inf, np.inf), (9.496, 0.390, 0.003)),
-        (ExGaussian(sigma=0.2), 9, 10, 0.8, (-np.inf, np.inf), (9.168, 0.423)),
+        (ExGaussian(), 9, 10, 0.8, (-np.inf, np.inf), (9.5, 0.390, 0)),
+        (ExGaussian(nu=0.2), 9, 10, 0.8, (-np.inf, np.inf), (9.319, 0.343)),
         (Exponential(), 0, 4, 0.9, (0, np.inf), (0.575)),
         (Gamma(), 0, 10, 0.7, (0, np.inf), (0.868, 0.103)),
         (Gamma(mu=9), 0, 10, 0.7, (0, np.inf), (2.170)),
         (Gumbel(), 0, 10, 0.9, (-np.inf, np.inf), (3.557, 2.598)),
         (Gumbel(mu=9), 0, 10, 0.9, (-np.inf, np.inf), (0.444)),
         (HalfCauchy(), 0, 10, 0.7, (0, np.inf), (5.095)),
         (HalfNormal(), 0, 10, 0.7, (0, np.inf), (9.648)),
         (HalfStudentT(), 1, 10, 0.7, (0, np.inf), (99.997, 7.697)),
         (HalfStudentT(nu=7), 1, 10, 0.7, (0, np.inf), (2.541)),
         (InverseGamma(), 0, 1, 0.99, (0, np.inf), (8.889, 3.439)),
-        (Kumaraswamy(), 0.1, 0.6, 0.9, (0, 1), (2.246, 7.427)),
+        (Kumaraswamy(), 0.1, 0.6, 0.9, (0, 1), (2.311, 7.495)),
         (Laplace(), -1, 1, 0.9, (-np.inf, np.inf), (0, 0.435)),
         (Laplace(mu=0.5), -1, 1, 0.9, (-np.inf, np.inf), (0.303)),
         (Logistic(), -1, 1, 0.5, (-np.inf, np.inf), (0, 0.91)),
         (LogNormal(), 1, 4, 0.5, (0, np.inf), (1.216, 0.859)),
         (LogNormal(mu=1), 1, 4, 0.5, (0, np.inf), (0.978)),
-        (LogitNormal(), 0.3, 0.8, 0.9, (0, 1), (0.226, 0.677)),
+        (LogitNormal(), 0.3, 0.8, 0.9, (0, 1), (0.213, 0.676)),
         (LogitNormal(mu=0.7), 0.3, 0.8, 0.9, (0, 1), (0.531)),
         (Moyal(), 0, 10, 0.9, (-np.inf, np.inf), (2.935, 1.6)),
         (Moyal(mu=4), 0, 10, 0.9, (-np.inf, np.inf), (1.445)),
         (Normal(), -1, 1, 0.683, (-np.inf, np.inf), (0, 1)),
         (Normal(), 10, 12, 0.99, (-np.inf, np.inf), (11, 0.388)),
         (Normal(mu=0.5), -1, 1, 0.8, (-np.inf, np.inf), (0.581)),
         (Pareto(), 1, 4, 0.9, (1, np.inf), (1.660, 1)),
         (Pareto(m=2), 1, 4, 0.9, (2, np.inf), (3.321)),
         (Rice(), 0, 4, 0.7, (0, np.inf), (0, 2.577)),
         (Rice(), 1, 10, 0.9, (0, np.inf), (3.453, 3.735)),
         (Rice(nu=4), 0, 6, 0.9, (0, np.inf), (1.402)),
-        (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (3.999, 3.647, 0)),
-        (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.2924, 4.905)),
+        (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (4.061, 3.648, -0.021)),
+        (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.293, 4.908)),
         (StudentT(), -1, 1, 0.683, (-np.inf, np.inf), (99.999, 0, 0.994)),
         (StudentT(nu=7), -1, 1, 0.683, (-np.inf, np.inf), (0, 0.928)),
         (
             Triangular(),
             0,
             4,
             0.8,
@@ -143,15 +143,15 @@
         (Weibull(alpha=2), 0, 10, 0.9, (0, np.inf), (6.590)),
         (BetaBinomial(), 2, 8, 0.9, (0, 8), (1.951, 1.345, 8)),
         (BetaBinomial(n=10), 2, 6, 0.6, (0, 10), (1.837, 2.181)),
         # # results for binomial are close to the correct result, but still off
         (Binomial(), 3, 9, 0.9, (0, 9), (9, 0.490)),
         (Binomial(n=12), 3, 9, 0.9, (0, 12), (0.612)),
         (DiscreteUniform(), -2, 10, 0.9, (-3, 11), (-2, 10)),
-        (DiscreteWeibull(), 1, 6, 0.7, (0, np.inf), (0.938, 1.604)),
+        (DiscreteWeibull(), 1, 6, 0.7, (0, np.inf), (0.939, 1.608)),
         (Geometric(), 1, 4, 0.99, (0, np.inf), (0.6837)),
         (HyperGeometric(), 2, 14, 0.9, (0, 21), (56, 21, 21)),
         (NegativeBinomial(), 0, 15, 0.9, (0, np.inf), (7.573, 2.077)),
         (NegativeBinomial(p=0.2), 0, 15, 0.9, (0, np.inf), (1.848)),
         (Poisson(), 0, 3, 0.7, (0, np.inf), (2.763)),
         (ZeroInflatedBinomial(), 1, 10, 0.9, (0, 10), (0.902, 9.0, 0.485)),
         (ZeroInflatedBinomial(psi=0.7), 1, 10, 0.7, (0, 11), (10, 0.897)),
```

### Comparing `preliz-0.5.0/preliz/tests/test_mle.py` & `preliz-0.6.0/preliz/tests/test_mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_optimization.py` & `preliz-0.6.0/preliz/tests/test_optimization.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,27 +8,31 @@
     Beta,
     Exponential,
     HalfNormal,
     Laplace,
     Normal,
     StudentT,
     Weibull,
+    Geometric,
+    Poisson,
 )
 
 
 @pytest.mark.parametrize(
     "p_dist, p_params",
     [
         (Beta, {"alpha": 2, "beta": 5}),
         (Exponential, {"beta": 3.7}),
         (HalfNormal, {"sigma": 2}),
         (Laplace, {"mu": 2.5, "b": 4}),
         (Normal, {"mu": 0, "sigma": 2}),
         (StudentT, {"nu": 5, "mu": 0, "sigma": 2}),
         (Weibull, {"alpha": 5.0, "beta": 2.0}),
+        (Geometric, {"p": 0.4}),
+        (Poisson, {"mu": 3.5}),
     ],
 )
 def test_find_ppf(p_dist, p_params):
     preliz_dist = p_dist(**p_params)
     x_vals = np.linspace(0.001, 0.999, 10)
     actual_ppf = preliz_dist.ppf(x_vals)
     expected_ppf = find_ppf(preliz_dist, x_vals)
```

### Comparing `preliz-0.5.0/preliz/tests/test_plots.py` & `preliz-0.6.0/preliz/tests/test_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,25 @@
         a_dist.plot_cdf(**kwargs)
         kwargs.pop("support", None)
         a_dist.plot_ppf(**kwargs)
 
 
 def test_plot_interactive():
     for idx, distribution in enumerate(pz.distributions.__all__):
-        if distribution not in ["Dirichlet", "MvNormal", "Truncated", "Censored"]:
+        if distribution not in ["Dirichlet", "MvNormal", "Truncated", "Censored", "Hurdle"]:
             dist = getattr(pz.distributions, distribution)
             kind = ["pdf", "cdf", "ppf"][idx % 3]
             xy_lim = ["auto", "both"][idx % 2]
             dist().plot_interactive(kind=kind, xy_lim=xy_lim)
         if distribution in ["Truncated", "Censored"]:
             dist = getattr(pz.distributions, distribution)
             dist(pz.Normal(0, 2), -1, 1).plot_interactive(kind="pdf", xy_lim="both")
+        if distribution == "Hurdle":
+            dist = getattr(pz.distributions, distribution)
+            dist(pz.Normal(0, 2), 0.9).plot_interactive(kind="pdf", xy_lim="both")
 
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {},
         {"marginals": True},
```

### Comparing `preliz-0.5.0/preliz/tests/test_quartile.py` & `preliz-0.6.0/preliz/tests/test_quartile.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 @pytest.mark.parametrize(
     "distribution, q1, q2, q3, result",
     [
         (AsymmetricLaplace(), -1, 1, 3, (1.0, 1.0, 2.885)),
         (Beta(), 0.3, 0.5, 0.7, (1.528, 1.528)),
         (Cauchy(), -1, 0, 1, (0, 1)),
         (ChiSquared(), 2, 4, 5.5, (4.329)),
-        (ExGaussian(), 8, 9, 10, (8.996, 1.482, 0.003)),
-        (ExGaussian(mu=8.5), 8, 9, 10, (1.401, 0.513)),
+        (ExGaussian(), 8, 9, 10, (9, 1.482, 0)),
+        (ExGaussian(mu=9), 8, 9, 10, (1.482, 0)),
         (Exponential(), 0.5, 1, 2.5, (0.611)),
         (Gamma(), 0.5, 1, 2.5, (0.894, 0.523)),
         (Gumbel(), 0.5, 1, 2.5, (0.751, 1.265)),
         (HalfCauchy(), 0.5, 1, 3, (1.105)),
         (HalfNormal(), 0.5, 1, 2, (1.613)),
         (HalfStudentT(), 0.5, 1, 2, (2.393, 1.311)),
         (InverseGamma(), 0.2, 0.3, 0.4, (3.881, 1.019)),
```

### Comparing `preliz-0.5.0/preliz/tests/test_roulette.py` & `preliz-0.6.0/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/tests/test_scipy.py` & `preliz-0.6.0/preliz/tests/test_scipy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 import pytest
 from numpy.testing import assert_almost_equal
 import numpy as np
 from scipy import stats
 
 
-from preliz.distributions import (
+from preliz import (
     AsymmetricLaplace,
     Beta,
+    BetaScaled,
+    Cauchy,
+    ChiSquared,
     DiscreteUniform,
+    ExGaussian,
     Exponential,
     Gamma,
+    Gumbel,
+    HalfCauchy,
     HalfNormal,
     HalfStudentT,
     InverseGamma,
+    Kumaraswamy,
     Laplace,
+    Logistic,
+    LogitNormal,
+    LogNormal,
+    Moyal,
     Normal,
+    Pareto,
+    Rice,
+    SkewNormal,
     StudentT,
     Triangular,
+    TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
     Bernoulli,
+    BetaBinomial,
     Binomial,
     Geometric,
+    HyperGeometric,
     NegativeBinomial,
     Poisson,
     ZeroInflatedBinomial,
     ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
 )
 
@@ -38,41 +55,83 @@
         (
             AsymmetricLaplace,
             stats.laplace_asymmetric,
             {"mu": 2.5, "b": 3.5, "kappa": 0.7},
             {"loc": 2.5, "scale": 3.5, "kappa": 0.7},
         ),
         (Beta, stats.beta, {"alpha": 2, "beta": 5}, {"a": 2, "b": 5}),
+        (
+            BetaScaled,
+            stats.beta,
+            {"alpha": 2, "beta": 5, "lower": -1, "upper": 3},
+            {"a": 2, "b": 5, "loc": -1, "scale": 4},
+        ),
+        (Cauchy, stats.cauchy, {"alpha": 2, "beta": 4.5}, {"loc": 2, "scale": 4.5}),
+        (ChiSquared, stats.chi2, {"nu": 3}, {"df": 3}),
+        (
+            ExGaussian,
+            stats.exponnorm,
+            {"mu": -1, "sigma": 0.5, "nu": 1},
+            {"loc": -1, "scale": 0.5, "K": 1 / 0.5},
+        ),
         (Exponential, stats.expon, {"beta": 3.7}, {"scale": 3.7}),
         (Gamma, stats.gamma, {"alpha": 2, "beta": 1 / 3}, {"a": 2, "scale": 3}),
+        (Gumbel, stats.gumbel_r, {"mu": 2.5, "beta": 3.5}, {"loc": 2.5, "scale": 3.5}),
+        (HalfCauchy, stats.halfcauchy, {"beta": 3.5}, {"scale": 3.5}),
         (HalfNormal, stats.halfnorm, {"sigma": 2}, {"scale": 2}),
         (
             HalfStudentT,
             stats.halfnorm,
             {"nu": 100, "sigma": 2},
             {"loc": 0, "scale": 2},
         ),  # not in scipy
         (InverseGamma, stats.invgamma, {"alpha": 5, "beta": 2}, {"a": 5, "scale": 2}),
+        (Kumaraswamy, stats.beta, {"a": 1, "b": 5}, {"a": 1, "b": 5}),  # not in scipy
         (Laplace, stats.laplace, {"mu": 2.5, "b": 4}, {"loc": 2.5, "scale": 4}),
+        (Logistic, stats.logistic, {"mu": 2.5, "s": 4}, {"loc": 2.5, "scale": 4}),
+        (LogNormal, stats.lognorm, {"mu": 0, "sigma": 2}, {"s": 2, "scale": 1}),
+        (LogitNormal, stats.beta, {"mu": 0, "sigma": 0.2}, {"a": 50.5, "b": 50.5}),  # not in scipy
+        (Moyal, stats.moyal, {"mu": 1, "sigma": 2}, {"loc": 1, "scale": 2}),
         (Normal, stats.norm, {"mu": 0, "sigma": 2}, {"loc": 0, "scale": 2}),
+        (Pareto, stats.pareto, {"m": 1, "alpha": 4.5}, {"b": 4.5}),
+        (
+            SkewNormal,
+            stats.skewnorm,
+            {"mu": 1, "sigma": 0.5, "alpha": 2},
+            {"a": 2, "loc": 1, "scale": 0.5},
+        ),
+        (Rice, stats.rice, {"nu": 0.5, "sigma": 2}, {"b": 0.25, "scale": 2}),
         (StudentT, stats.t, {"nu": 5, "mu": 0, "sigma": 2}, {"df": 5, "loc": 0, "scale": 2}),
         (Triangular, stats.triang, {"lower": 0, "upper": 1, "c": 0.45}, {"c": 0.45}),
+        (
+            TruncatedNormal,
+            stats.truncnorm,
+            {"mu": 0, "sigma": 1, "lower": -1, "upper": 1},
+            {"loc": 0, "scale": 1, "a": -1, "b": 1},
+        ),
         (Uniform, stats.uniform, {"lower": -2, "upper": 1}, {"loc": -2, "scale": 3}),
         (VonMises, stats.vonmises, {"mu": 0, "kappa": 10}, {"loc": 0, "kappa": 10}),
         (Wald, stats.invgauss, {"mu": 2, "lam": 10}, {"mu": 2 / 10, "scale": 10}),
         (
             Weibull,
             stats.weibull_min,
             {"alpha": 5.0, "beta": 2.0},
             {"c": 5.0, "scale": 2.0},
         ),
         (Binomial, stats.binom, {"n": 4, "p": 0.4}, {"n": 4, "p": 0.4}),
+        (
+            BetaBinomial,
+            stats.betabinom,
+            {"alpha": 2, "beta": 5, "n": 10},
+            {"n": 10, "a": 2, "b": 5},
+        ),
         (Bernoulli, stats.bernoulli, {"p": 0.4}, {"p": 0.4}),
         (DiscreteUniform, stats.randint, {"lower": -2, "upper": 1}, {"low": -2, "high": 2}),
         (Geometric, stats.geom, {"p": 0.4}, {"p": 0.4}),
+        (HyperGeometric, stats.hypergeom, {"N": 50, "k": 10, "n": 25}, {"M": 50, "N": 25, "n": 10}),
         (
             NegativeBinomial,
             stats.nbinom,
             {"mu": 3.5, "alpha": 2.1},
             {"n": 2.1, "p": 2.1 / (3.5 + 2.1)},
         ),
         (Poisson, stats.poisson, {"mu": 3.5}, {"mu": 3.5}),
@@ -104,25 +163,36 @@
     if preliz_name != "VonMises":
         # for the VonMises we used the differential entropy definition.
         # SciPy uses a different one
         actual = preliz_dist.entropy()
         expected = scipy_dist.entropy()
         if preliz_dist.kind == "discrete":
             assert_almost_equal(actual, expected, decimal=1)
-        elif preliz_name == "HalfStudentT":
+        elif preliz_name in [
+            "HalfStudentT",
+            "Moyal",
+            "LogitNormal",
+            "SkewNormal",
+            "Rice",
+            "ExGaussian",
+        ]:
             assert_almost_equal(actual, expected, decimal=2)
         else:
             assert_almost_equal(actual, expected, decimal=4)
 
     rng = np.random.default_rng(1)
     actual_rvs = preliz_dist.rvs(20, random_state=rng)
     rng = np.random.default_rng(1)
     expected_rvs = scipy_dist.rvs(20, random_state=rng)
     if preliz_name in [
+        "ExGaussian",
         "HalfStudentT",
+        "Kumaraswamy",
+        "LogitNormal",
+        "Moyal",
         "StudentT",
         "Weibull",
         "InverseGamma",
         "DiscreteUniform",
         "ZeroInflatedBinomial",
         "ZeroInflatedNegativeBinomial",
         "ZeroInflatedPoisson",
@@ -137,57 +207,67 @@
 
     actual_pdf = preliz_dist.pdf(actual_rvs)
     if preliz_dist.kind == "continuous":
         expected_pdf = scipy_dist.pdf(actual_rvs)
     else:
         expected_pdf = scipy_dist.pmf(actual_rvs)
 
-    if preliz_name == "HalfStudentT":
+    if preliz_name == "LogitNormal":
+        assert_almost_equal(actual_pdf, expected_pdf, decimal=1)
+    elif preliz_name == "HalfStudentT":
         assert_almost_equal(actual_pdf, expected_pdf, decimal=2)
     else:
         assert_almost_equal(actual_pdf, expected_pdf, decimal=4)
 
     support = preliz_dist.support
     cdf_vals = np.concatenate([actual_rvs, support, [support[0] - 1], [support[1] + 1]])
 
     actual_cdf = preliz_dist.cdf(cdf_vals)
     expected_cdf = scipy_dist.cdf(cdf_vals)
 
-    if preliz_name == "HalfStudentT":
+    if preliz_name in ["HalfStudentT", "LogitNormal"]:
         assert_almost_equal(actual_cdf, expected_cdf, decimal=2)
     else:
         assert_almost_equal(actual_cdf, expected_cdf, decimal=6)
 
     x_vals = [-1, 0, 0.25, 0.5, 0.75, 1, 2]
     actual_ppf = preliz_dist.ppf(x_vals)
     expected_ppf = scipy_dist.ppf(x_vals)
-    if preliz_name in ["HalfStudentT", "Wald"]:
+    if preliz_name in ["HalfStudentT", "Wald", "LogitNormal", "SkewNormal", "ExGaussian"]:
         assert_almost_equal(actual_ppf, expected_ppf, decimal=2)
     else:
         assert_almost_equal(actual_ppf, expected_ppf)
 
     actual_logpdf = preliz_dist.logpdf(actual_rvs)
     if preliz_dist.kind == "continuous":
         expected_logpdf = scipy_dist.logpdf(actual_rvs)
     else:
         expected_logpdf = scipy_dist.logpmf(actual_rvs)
+
     if preliz_name == "HalfStudentT":
         assert_almost_equal(actual_logpdf, expected_logpdf, decimal=0)
+    elif preliz_name == "LogitNormal":
+        assert_almost_equal(actual_logpdf, expected_logpdf, decimal=1)
+    elif preliz_name in ["SkewNormal"]:
+        assert_almost_equal(actual_logpdf, expected_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_logpdf, expected_logpdf)
 
     actual_neg_logpdf = preliz_dist._neg_logpdf(actual_rvs)
     expected_neg_logpdf = -expected_logpdf.sum()
-    if preliz_name == "HalfStudentT":
+    if preliz_name in ["HalfStudentT", "LogitNormal"]:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=1)
+    elif preliz_name in ["TruncatedNormal", "SkewNormal"]:
+        assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf, decimal=6)
     else:
         assert_almost_equal(actual_neg_logpdf, expected_neg_logpdf)
 
     if preliz_dist.__class__.__name__ not in [
         "HalfStudentT",
+        "Rice",
         "VonMises",
         "ZeroInflatedBinomial",
         "ZeroInflatedNegativeBinomial",
         "ZeroInflatedPoisson",
     ]:
         actual_moments = preliz_dist.moments("mvsk")
         expected_moments = scipy_dist.stats("mvsk")
@@ -199,19 +279,23 @@
         actual_moments = preliz_dist.moments("m")
         expected_moments = scipy_dist.stats("m")
 
     else:
         actual_moments = preliz_dist.moments("mv")
         expected_moments = scipy_dist.stats("mv")
 
-    if preliz_name == "HalfStudentT":
+    if preliz_name in ["HalfStudentT", "LogitNormal"]:
         assert_almost_equal(actual_moments, expected_moments, decimal=1)
+    elif preliz_name in ["TruncatedNormal"]:
+        assert_almost_equal(actual_moments, expected_moments, decimal=6)
     else:
         assert_almost_equal(actual_moments, expected_moments)
 
     actual_median = preliz_dist.median()
     expected_median = scipy_dist.median()
 
     if preliz_name == "HalfStudentT":
         assert_almost_equal(actual_median, expected_median, decimal=1)
+    elif preliz_name == "SkewNormal":
+        assert_almost_equal(actual_median, expected_median, decimal=6)
     else:
         assert_almost_equal(actual_median, expected_median)
```

### Comparing `preliz-0.5.0/preliz/tests/test_special.py` & `preliz-0.6.0/preliz/tests/test_special.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pytest
+# pylint: disable=no-member
 from numpy.testing import assert_almost_equal
 import numpy as np
 
 from scipy import special as sc_special
 from preliz.internal import special as pz_special
 
 
@@ -53,7 +53,17 @@
     x = np.linspace(0.1, 10, 100)
     assert_almost_equal(sc_special.gamma(x), pz_special.gamma(x))
 
 
 def test_digamma():
     x = np.linspace(0.1, 10, 100)
     assert_almost_equal(sc_special.digamma(x), pz_special.digamma(x))
+
+
+def test_logit():
+    x = np.linspace(-0.1, 1.1, 100)
+    assert_almost_equal(sc_special.logit(x), pz_special.logit(x))
+
+
+def test_expit():
+    x = np.linspace(-20, 10, 500)
+    assert_almost_equal(sc_special.expit(x), pz_special.expit(x))
```

### Comparing `preliz-0.5.0/preliz/tests/test_truncated.py` & `preliz-0.6.0/preliz/tests/test_truncated.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,17 @@
     assert_almost_equal(actual_mean, expected_mean, decimal=2)
 
     actual_var = custom_truncnorm_dist.var()
     expected_var = genera_truncnorm_dist.var()
     assert_almost_equal(actual_var, expected_var, decimal=2)
 
     actual_skew = custom_truncnorm_dist.skewness()
-    expected_skew = genera_truncnorm_dist.rv_frozen.stats("s")
+    expected_skew = genera_truncnorm_dist.skewness()
     assert_almost_equal(actual_skew, expected_skew, decimal=2)
 
     actual_kurt = custom_truncnorm_dist.kurtosis()
-    expected_kurt = genera_truncnorm_dist.rv_frozen.stats("k")
+    expected_kurt = genera_truncnorm_dist.kurtosis()
     assert_almost_equal(actual_kurt, expected_kurt, decimal=1)
 
     actual_entropy = custom_truncnorm_dist.entropy()
-    expected_entropy = genera_truncnorm_dist._entropy()
+    expected_entropy = genera_truncnorm_dist.entropy()
     assert_almost_equal(actual_entropy, expected_entropy, decimal=2)
```

### Comparing `preliz-0.5.0/preliz/unidimensional/beta_mode.py` & `preliz-0.6.0/preliz/unidimensional/beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/unidimensional/dirichlet_mode.py` & `preliz-0.6.0/preliz/unidimensional/dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/unidimensional/maxent.py` & `preliz-0.6.0/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/unidimensional/mle.py` & `preliz-0.6.0/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/unidimensional/quartile.py` & `preliz-0.6.0/preliz/unidimensional/quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/unidimensional/quartile_int.py` & `preliz-0.6.0/preliz/unidimensional/quartile_int.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/preliz/unidimensional/roulette.py` & `preliz-0.6.0/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/pyproject.toml` & `preliz-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `preliz-0.5.0/PKG-INFO` & `preliz-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.5.0
+Version: 0.6.0
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
```

