# Module 09: Machine Learning: Models of Models - Surrogates and Emulators

## 1. Introduction and Overview

In this module we explore how we can use machine learning (ML) methods to create _emulators_, also called surrogate models. An emulator is essentially a model of a model. That is, it is an ML-based model that is designed to mimic the behavior of a different model, given similar inputs as that model. Specifically, we will use two alternative ML-based approaches, `XGBoost` (an ensemble of weak learners) and `MLPRegressor` (a neural network-based models) to create an emulator of the Snow-17 temperature index-based snow accumulation and melt model.

## 2. Why Emulation?

"Why would we need a model of a model?" is a very good question. In our case the Snow-17 model is very computationally inexpensive and conceptually simple. However, there are many cases in which our model is much more sophisticated and computationally expensive. Moreover, in some cases we're not interested in __*all*__ of the outputs of a model, but only a small subset. For example, my research group uses the [Weather Research and Forecasting](https://www.mmm.ucar.edu/models/wrf) (WRF) model. WRF is a numerical weather prediction model that simulates the 4-D evolution of the coupled land-atmosphere system. As such it generates __*a lot*__ of output data and is very computationally expensive for anything more than a very short run over a limited area. As hydrologists, however, we are frequently most interested in WRF's predictions at the bottom of the atmosphere – i.e., the land surface. We are interested in precipitation, temperature, humidity, and solar and thermal radiation fluxes simulated by WRF - the surface hydrometeorology. It would be very nice if we could have a  model that: (1) approximately reproduced the surface hydrometeorology that WRF would simulate given the same inputs, (2) ran in a fraction of the time of the full WRF model, and (3) output only those variables we're interested in and maybe some other diagnostic variables. This is where emulation comes in! If we have a sufficiently large dataset of surface hydrometeorology output from long WRF runs (we do! See this paper by [Rudisill et al.](https://gmd.copernicus.org/articles/16/6531/2023/gmd-16-6531-2023.html)) on which we can train a ML model, we can create an __*emulator*__ of WRF.   
 

## 3. An Emulation Example: Parameter Estimation

A related use of emulators is when we need to calibrate some parameters of the model, but running the full model many times to explore a large parameter space is computationally too expensive. We can:

1. Run the model for a limited number of runs with a smaller set of the larger parameter space (we should be careful in how we create that smaller subset of parameters),
2. Train an ML model on that smaller subset of runs making sure to expose the ML model to the values and combinations of the parameters that were used to do those runs, and 
3. Use the emulator to explore a larger portion of the parameter space, confront those emulator predictions with observational data, and select one or a small number of parameter combinations that perform best against some performance metric. 

That's what we will be doing in this module. This module consists of three notebooks:

1. [`mod09-Snow17-ensemble-run.ipynb`](./mod09-Snow17-ensemble-run.ipynb): A notebook that sets up and executes a number of runs with the Snow-17 model in the East River watershed in Colorado for a user-defined number of parameter combinations and ranges of parameters. The output of this notebook is a set of simulated SWE time series for each parameter combination.
2. ['mod09-Snow17-xgb-emulator-training.ipynb](./mod09-Snow17-xgb-emulator-training.ipynb): A notebook that takes the output from the Snow-17 model runs, trains an ensemble of weak learners ML emulator, and evaluates the emulator against Snow-17 simulations that were not used in the training process.
3. ['mod09-Snow17-NN-emulator-training.ipynb'](./mod09-Snow17-NN-emulator-training.ipynb): A notebook similar to the one above, but that uses a neural network-based ML model, instead.