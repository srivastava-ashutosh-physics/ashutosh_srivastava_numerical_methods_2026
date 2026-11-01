# Ashutosh Srivastava — Numerical Methods Assignment 3 (Q2 and Q4)

**Assessment scope:** Question 2 (32 marks) and Question 4 (76 marks) only.  
**Total assessed:** 108 marks.

## Question 2 — 31/32

| Part | Maximum | Awarded | Comments |
|---|---:|---:|---|
| Q2.1 Define `f(x)` | 2 | 2 | Correct implementation of the cubic function. |
| Q2.2 Analytic derivative | 2 | 2 | Correct derivative, \(f'(x)=(x-1)(3x-5)\). |
| Q2.3 Define `w(x)=f(x)/f'(x)` | 2 | 2 | Correctly simplifies the ratio to \((x-1)(x-2)/(3x-5)\), with the appropriate domain caveat. |
| Q2.4A Plot and show the same roots | 3 | 3 | Correctly plots both functions, splits the plot at the pole and marks the shared roots. |
| Q2.4B Show the double root becomes simple | 2 | 2 | Correctly identifies that cancellation reduces the multiplicity at x=1 from two to one. |
| Q2.5 Explain the apparent crossing at x=5/3 | 5 | 5 | Correct one-sided limits and explanation that x=5/3 is a vertical asymptote, not a root. |
| Q2.6 Implement Newton's method | 4 | 3 | Correct Newton update and prescribed relative-step stopping criterion. It raises an error for a near-zero derivative, but does not check for non-finite iterates or explicitly distinguish reaching the iteration limit from convergence. |
| Q2.7 Find all roots of `f` | 4 | 4 | Correctly finds x=1 and x=2 from suitable initial guesses. |
| Q2.8 Find all roots of `w` | 4 | 4 | Correctly finds both roots, x=1 and x=2. |
| Q2.9 Compare convergence at x=1 | 4 | 4 | Correctly explains linear convergence for the double root of f and quadratic convergence for the simple root of w; the iteration history supports the comparison. |
| **Q2 total** | **32** | **31** | |

## Question 4 — 59/76

| Part | Maximum | Awarded | Comments |
|---|---:|---:|---|
| Q4.1 Load data using pandas | 2 | 2 | Correctly loads the supplied CSV and extracts the two data columns. |
| Q4.2 Plot data and estimate A and C | 6 | 6 | Correct plot and sensible peak-based estimates for A and C. |
| Q4.3 Choose B and plot the initial model | 6 | 6 | Compares several B values and selects a plausible initial parameter vector. |
| Q4.4 Implement first central difference | 6 | 6 | Correct central-difference formula. |
| Q4.5 Calculate sum of squared residuals | 6 | 6 | Correct objective function. |
| Q4.6 Calculate gradient G | 8 | 8 | Correct central finite-difference construction of the gradient. |
| Q4.7 Calculate Jacobian of G | 8 | 8 | Correct central finite-difference construction of the Jacobian. |
| Q4.8 Implement multidimensional Newton solver | 12 | 8 | Correctly forms the Newton system and handles a singular linear solve. However, there is no damping/line search, parameter constraints, or robust finite-value check. The same very small finite-difference step is used for all three differently scaled parameters, and the solver can accept a numerically vanishing gradient even when far from a minimum. |
| Q4.9 Run solver and report solution | 8 | 0 | The run is not a valid convergence. It reports \(\|G\|=0\) at \(A\\approx135578\), \(B\\approx0.366\), \(C\\approx140\), while the residual sum remains about \(3.29\\times10^7\). This is a false convergence caused by numerical underflow/insensitivity when the fitted peak is far outside the data interval. |
| Q4.10 Plot data, initial guess and best-fit model | 8 | 5 | Includes the observations, initial model and a labelled final curve, but the final curve is based on the invalid, non-converged parameter values and is not a best fit to the data. |
| Q4.11 Test other initial guesses and discuss convergence | 6 | 4 | Tests multiple starting guesses and correctly observes failures and sensitivity to initialization. However, the discussion does not catch the false convergence in the main run, and one of the alternative runs produces non-finite values without a robust stop condition. |
| **Q4 total** | **76** | **59** | |

## Overall

| Question | Maximum | Awarded |
|---|---:|---:|
| Q2 | 32 | 31 |
| Q4 | 76 | 59 |
| **Total** | **108** | **90** |

**Final score: 90/108**


