# Here is a quick summary of Botta's research and some background on HAR models: 
* Botta (2026) argues that Heterogeneous AutoRegressive (HAR) Models can capture multi-horizon volatility dynamics in financial markets
* The long-memory process of financial volatility is approximated with a simple autoregressive structure across multiple time scales
* Volatility is characterized by a cascade structure, i.e. short-term volatility affects medium-term volatility and so on.
* In the model, an intercept(beta_0), daily (beta_1), weekly (beta_2), and monthly (beta_3) volatility persistence parameters and an error term are used 
* A Bayesian framework is used here to prevent overfitting due to correlated regressors and to quantify uncertainty in voltatility persistence parameters
* Beta is modelled as multivariate normal and sigma^2 (the error variance) is modelled as inverse gamma
* A Gibbs sampler is used to compute posterior mean estimates for the 3 persistence parameters as well as the variance of the errors

# I replicated his HAR model and added MCMC algorithm diagnostics. 
# Moreover, I added a continuous integration continuous deployment (CICD) workflow through Github actions and automated the knitting of the R Markdown file to HTML.




# References: 
Botta, C. (2026, April 13). "Bayesian HAR Models - Heterogeneous AutoRegressive Models for Volatility Forecasting". Linkedin. https://www.linkedin.com/feed/update/urn:li:activity:7408897863520268288/?originTrackingId=GUdsm4qcTRyI%2BWrMFt5Gmg%3D%3D.
