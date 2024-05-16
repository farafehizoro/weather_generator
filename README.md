# WEATHER GENERATOR 
```
from weather_generator import Rain_WeatherGenerator

rain_WG = Rain_WeatherGenerator()
rain_WG.import_data(data_list= rain_data, start_date= "1991-01-01", end_date= "2020-12-31")
daily_rain_generated = rain_WG.run_weath_gen(2024, month=02, nb_real=100, rain_occ_model= "mixed_order", rain_quant_model= "gamma"):

```

Stochastic generation of daily weather data. 

# About
This package is a stochatic weather generator, that create daily weather data. For now, the method work for rainfall data.

The data needed for the calculation are:
* historical daily weather data that should be for at least 30 years.


For daily rainfall generation, different method (type of model) are avalaible from which the users can choose: 
* rain occurrence model:  one order markov chain, second order markov chain, mixed order markov chain
* daily rain quantity model:  weibull, exponential, gamma, hyperexponential (sum of 2 exponential distribution)
The input data must have the same timestep and length.

# Install
```
pip install weather_generator 
```