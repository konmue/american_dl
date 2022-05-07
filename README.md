# Regression and Deep Learning approaches for pricing American Options

Implementation of different algorithms to price a Bermudan Option.

Including:
* Least-Squares Monte Carlo (LSM) with different features:
	* just the path and payoff (for illustration purposes)
	* features suggested by Longstaff & Schwartz (2001)
	* features generated by an untrained MLP ("random neural network") as suggested by Herrera et al. (2021)
* Deep LSM approach as suggested by Becker et al. (2020), i.e., using a trained MLP as the feature map for LSM
* Deep Optimal Stopping (DOS) as suggested by Becker et al. (2019) that directly parametrizes the stopping decision with neural networks

***
* Results are shown for pricing a Bermudan Max Call for different combinations of number of assets and initial values in a Black-Scholes type market. I.e., asset prices are assumed to be uncorrelated geometric brownian motions.
* Results include approximations of both the lower and upper bound for the price.

***
Reference papers:
* [Valuing American Options by Simulation:
A Simple Least-Squares Approach](https://people.math.ethz.ch/~hjfurrer/teaching/LongstaffSchwartzAmericanOptionsLeastSquareMonteCarlo.pdf)
* [Deep optimal stopping](https://arxiv.org/pdf/1804.05394.pdf)
* [ Pricing and Hedging American-Style Options with Deep Learning](https://www.mdpi.com/1911-8074/13/7/158/htm)
* [Optimal Stopping via Randomized Neural Networks](https://arxiv.org/abs/2104.13669)
