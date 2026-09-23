Few Notes:

Data Set : This is not a new dataset, but it demonstrates how powerful the Heston model can be when it comes to equity option valuation. There are quite a few simplifying assumptions in the analysis—apologies for that. I didn’t have enough time to incorporate interest rates and some of the other inputs properly.

Optimization/Calibration : DEoptim package is used to calibrate the parameters. DEoptim implements Differential Evolution (DE), which is a global optimization algorithm inspired by evolutionary processes. It searches for parameter values that minimize or maximize an objective function without requiring derivatives. I acknowledge that the way better calibration is possible. But the result was pretty good; and there was no reason to go for fancy machine learning stuff.

Why this matters: Once we have calibrated the model parameters, we can use them to simulate the underlying stochastic process. The same parameter set can also be used to price different types of options.
