
<!-- README.md is generated from README.Rmd. Please edit that file -->
\#tidyforecast
==============

[![Travis build status](https://travis-ci.org/tidyverts/tidyforecast.svg?branch=master)](https://travis-ci.org/tidyverts/tidyforecast) [![Licence](https://img.shields.io/badge/licence-GPL--3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)

The R package *fable* provides methods and tools for displaying and analysing univariate time series forecasts including exponential smoothing via state space models and automatic ARIMA modelling. Data, model and forecast objects are all stored in a tidy format.

Installation
------------

You can install the **development** version from [Github](https://github.com/tidyverts/tidyforecast)

``` r
# install.packages("devtools")
devtools::install_github("tidyverts/tidyforecast")
```

Example
-------

``` r
library(fable)
library(tsibbledata)
UKLungDeaths %>%
  ETS(log(mdeaths)) %>%
  forecast %>%
  autoplot
```
