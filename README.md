# Package: fitdistrib

R package for fitting probability distributions to flood data at NVE

# Installation

On RStudio, install package devtools:

> install.packages("devtools")

Afterwards, run these commands:

> library(devtools)

> install_github("fbaffie/fitdistrib")

# Example

The following example fit the generalized extreme value distribution with the MLE method 
using a randomly generated dataset based on the same distribution

> library(fitdistrib)

> gev_mle(evd::rgev(10000, loc=0, scale=1, shape=0))
