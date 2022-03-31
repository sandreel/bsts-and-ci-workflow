# bsts-and-ci-workflow

This notebook contains some experiments about fitting Bayesian structural time series using

* the bsts R package (https://CRAN.R-project.org/package=bsts by Steven L. Scott) and
* the CausalImpact R package (CausalImpact 1.2.1, Brodersen et al., Annals of Applied Statistics (2015), http://google.github.io/CausalImpact/) which builds on bsts and enables the analysis of the causal impact of an intervention on a time series.

The goal of this notebook is to compare workflows and results, not to achieve the best fit possible. I am fitting one model with a local level and a seasonality component, these components can easily be included into the CausalImpact workflow, using default parameters. In addition, I test a model with an autoregressive and a seasonality component, therefore I need to feed a custom bsts model into CausalImpact. This was a learning exercise I did - maybe it is useful to others. Comments and corrections are welcome.
