# HMM Applied to Intraday Momentum Trading with Side Information

## Description
* Predicted 1-step signal magnitude to observe the performance of simple momentum strategy in HMM framework and IOHMM framework when side information like seasonality and volatility are introduced using spline methods.

## Abstract (From First Reference)
* A Hidden Markov Model for intraday momentum trading is presented which specifies a latent momentum state responsible for generating the observed securities’ noisy returns.
* Existing momentum trading models suffer from time-lagging caused by the delayed frequency response of digital filters. Time-lagging results in a momentum signal of the wrong sign, when the market changes trend direction. A key feature of this state space formulation, is no such lagging occurs, allowing for accurate shifts in signal sign at market change points.
* An Input Output Hidden Markov Model is used to incorporate these univariate predictive signals into the transition matrix, presenting a possible solution for dealing with the signal combination problem.
* Bayesian inference is then carried out to predict the securities t + 1 return using the forward algorithm. The model is simulated on one year’s worth of e-mini SP500 futures data at one minute sampling frequency, and it is shown that pre-cost the models have a Sharpe ratio in excess of 2.0.

## Notes
* The original data used in this project is the TAQ tick data of AAPL (approximately 70G) in 2020 from NYSE, which is purchased by our department. Please try to find a way to get the corresponding data if you want to run the code of Data.ipynb. Sorry for the inconvenience.
* The code of Spline is the most computationally intensive part, which took about 6 hours on my PC.
* In this report/slides, the parts of Hidden Markov Model Basics (PART2) and Numerical Results (PART5) are not given.
    * Hidden Markov Model Basics (PART2) can be found in ./Display/Hidden_Markov_Model_Basics.html
    * Numerical Results (PART5) can be found in other .ipynb and .html files

## Main Reference
* <a style='color: black;' href='https://econpapers.repec.org/paper/arxpapers/2006.08307.htm' target='_blank'>https://econpapers.repec.org/paper/arxpapers/2006.08307.htm</a>
* <a style='color: black;' href='http://www.tup.tsinghua.edu.cn/booksCenter/book_08132901.html' target='_blank'>http://www.tup.tsinghua.edu.cn/booksCenter/book_08132901.html</a>
* <a style='color: black;' href='https://ieeexplore.ieee.org/document/18626?arnumber=18626' target='_blank'>https://ieeexplore.ieee.org/document/18626?arnumber=18626</a>
