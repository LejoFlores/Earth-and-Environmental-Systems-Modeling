# Module 03 Code: 1-D Diffusion Problems

## Content

In this folder you will find the following Jupyter notebooks for review simulation of 1-D diffusive problems using:

* Explicit methods,
* Implicit method, and
* Crank-Nicolson method.

The specific model that we develop in this module is a model of temperature diffusion in permafrost. We use synthetic, but realistic, values for soil density, thermal conductivity, and heat capacity and simulate the vertical distribution of soil temperature in response to periodic air temperatures at the surface. We are specifically interested in the depth of the soil that annually warms to a temperature of 0 °C (thawing), a depth that is referred to as the "active layer" in the study of permafrost. In the assignment, students extend this model to evaluate how the active layer thickness changes with warming air temperatures associated with climate change. 

You will also find the following notebooks:

* [mod03_1D-Diffusion-ExplicitExample.ipynb](./mod03_1D-Diffusion-ExplicitExample.ipynb): This notebook develops a solution to the soil heat diffusion problem using an explicit solving scheme. 
* [mod03_1D-Diffusion-ImplicitExample.ipynb](./mod03_1D-Diffusion-ImplicitExample.ipynb): This notebook develops a solution to the soil heat diffusion problem using an implicit solving scheme. 
* [mod03_1D-Diffusion-CNExample.ipynb](./mod03_1D-Diffusion-CNExample.ipynb): This notebook develops a solution to the soil heat diffusion problem using the Crank-Nicolson solving scheme that uses both an explicit and implicit approaches. 


