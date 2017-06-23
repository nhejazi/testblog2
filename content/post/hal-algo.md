+++
date = "2017-06-22"
author = "Nima Hejazi"
title = "the highly adaptive LASSO estimator"
summary = "Discussion of HAL's statistical properties, and speeding it up"
categories = [ "statistics", "machine learning", "computing" ]
comments = false
draft = true

+++

## The Highly Adaptive LASSO (HAL)

Recent developments in statistical machine learning and causal inference led to
a very interesting new estimation algorithm (called the highly adaptive LASSO)
being proposed by D.C. Benkeser and M.J. van der Laan. Due to the intensive
nature of this estimation algorithm, it can take quite a long time to run,
becoming infeasible rather quickly, as the dimensionality of a data set of
interest grows. Initial plans included integrating `hal` with `rcpp` in order to
boost performance, which would require that parts of the `hal` codebase be
re-written in C++ via the Rcpp framework. I thought `renjin` might be able to
help out with this. Here goes:

```{r}
library(hal)
```

To be continued...
