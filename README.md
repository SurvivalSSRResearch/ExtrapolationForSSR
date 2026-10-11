# Adaptive Sample Size Re-Estimation Using Survival Extrapolation Methods
## Overview

This repository contains R simulation programs developed to evaluate survival extrapolation methods for adaptive sample size re-estimation (SSR) based on unblinded interim analyses in clinical trials with time-to-event endpoints.

The simulation study generates survival data from piecewise Weibull and piecewise log-normal distributions, applies extrapolation methods to predict survival outcomes beyond the interim analysis, performs SSR, and evaluates the methods in terms of Type I error, statistical power, probability and magnitude of sample size increases, power gain efficiency, and accuracy of survival estimates.

## Simulation Designs

Two study designs are evaluated:

- **Fixed-events design:** The study ends when a predetermined number of events is reached.
- **Fixed follow-up design:** Each subject ends the study at the earlier of: 1) event onset; 2) pre-defined follow-up duration is reached. 

Simulation scenarios are evaluated under both the null hypothesis (H₀) and alternative hypothesis (H₁), using various underlying survival distributions and hazard patterns.

## Survival Extrapolation Methods

The simulation programs evaluate 24 survival extrapolation methods, including:

- Nonparametric Kaplan–Meier (KM) approaches
- Fully parametric survival models
- Piecewise parametric models
- Hybrid KM and parametric extrapolation methods
- Flexible spline-based survival models

Parametric and hybrid models are based on the exponential, Weibull, gamma, log-logistic, and log-normal distributions.

## Evaluation Measures

The performance of the extrapolation methods is evaluated using:

- Statistical power and power gain
- Type I error
- Probability of sample size increase
- Magnitude of sample size increase
- Power gain per proportional event increase
- Relative root mean squared error (RMSE) of restricted mean survival time (RMST)

## Software

The simulation programs are written in R Markdown (.Rmd) using the rmarkdown package (version 2.29).

## Usage

The programs are organized according to study design, hypothesis setting, and extrapolation method.

## Citation

If you use these programs in academic research, please cite the associated manuscript when its bibliographic details become available.

## License

No open-source license is currently provided. All rights are reserved unless otherwise specified.
