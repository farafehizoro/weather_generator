# WEATHER GENERATOR 
```
To update
```

Stochastic generation of daily weather data. 

# About
This package is a stochatic weather generator, that create daily weather data. For now, the method work for rainfall data.

The data needed for the calculation are:
* historical daily weather data for at least 30 years.


For daily rainfall generation, different method (type of model) are avalaible from which the users can choose: 
* rain occurrence model:  one order markov chain, second order markov chain, mixed order markov chain
* daily rain quantity model:  weibull, exponential, gamma, hyperexponential (sum of 2 exponential distribution)
The input data must have the same timestep and length.

# Install
```
pip install weather_generator 
```