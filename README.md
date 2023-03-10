# Tolerance Intervals: Python
Python package for tolerance intervals. Derived from: Derek S. Young (2010). tolerance: An R Package for Estimating Tolerance Intervals. Journal of Statistical Software, 36(5), 1-39. URL http://www.jstatsoft.org/v36/i05/.

"Description: Statistical tolerance limits provide the limits between which we can expect to find a specified proportion of a sampled population with a given level of confidence.  This package provides functions for estimating tolerance limits (intervals) for various univariate distributions (binomial, Cauchy, discrete Pareto, exponential, two-parameter exponential, extreme value, hypergeometric, Laplace, logistic, negative binomial, negative hypergeometric, normal, Pareto, Poisson-Lindley, Poisson, [Rayleigh], uniform, and Zipf-Mandelbrot), Bayesian normal tolerance limits, multivariate normal tolerance regions, nonparametric tolerance intervals, tolerance bands for regression settings (linear regression, nonlinear regression, nonparametric regression, and multivariate regression), and analysis of variance tolerance intervals." (Derek Young)

The package answers the practical question: "I have (1-α)*100% confidence that (P)*100% of my population falls within certain bounds."

- One sided and two sided tolerance intervals are available for nearly every tolerance interval. 

Notes:
- The gamtolint and cautolint files are slightly different than the R equivalent, this is due to R using the Newton minimization method and the Python code uses the Quasi Newton BFGS minimization method. Both methods use nonlinear minimization. The Quasi Newton method does not require solving a linear system of equations, it does not require a second derivative, and it's faster relative to the Newton method. One downside of the Quasi Newton method as opposed to the Newton method is that the Quasi Newton method has a less precise convergence path. 
- npmvtolregion may have some unknown errors. 
