# Bayesian Home Valuer

Bayesian linear regression model to predict house sale prices using **JAGS** (Just Another Gibbs Sampler) and **Student-t** errors for robustness against outliers.

## Highlights
- MCMC sampling with runjags (3 chains, diagnostics: trace, density, autocorrelation, Gelman-Rubin, ESS)
- Posterior predictive checks
- 95% Highest Density Intervals (HDI) for predictions
- Predictions for 5 hypothetical properties

## Tech Stack
- R + JAGS
- Packages: ggplot2, ggpubr, rjags, runjags, ks, coda
- Reproducible via R Markdown

## How to Run
1. Install JAGS: https://mcmc-jags.sourceforge.io/
2. `install.packages(c("rjags", "runjags", "ggplot2", "ggpubr", "coda"))`
3. Open `ABS2.Rmd` in RStudio and knit

## Key Findings
- Area has the strongest positive effect (prior centered at 90)
- PropertyType shows negative impact (prior -150k)
- Model robust to outliers thanks to Student-t likelihood

## View the Report
- [PDF version](ABS2.pdf) ← direct link works on GitHub

Built by Arka • Melbourne • 2026  
Part of my data science / Bayesian portfolio