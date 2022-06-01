
[![describtor - e.g. python version](https://img.shields.io/badge/R%20Studio-Version%201.4-9cf)](www.desired_reference.com)


# Hidden Markov Modelling: How does the plant based market grow? 
----- 

<div align="center"><img src="https://github.com/Orlz/Hidden_Markov_Modelling/blob/main/supplementary_material/vegan.png"width = 100/></div>

The global plant-based food market has experienced rapid growth over the past five years, with many consumers opting to reduce their meat and dairy consumption under the principle of a more sustainable future. 
This conscious choice has been felt within the food market as an upsurge in demand for plant-based products coupled with a notable increase in government funding into the plant protein industry. This 2-fold study looks at how the plant-based food market has evolved in Denmark and how non-vegetarian households have been adopting plant-based products. 
Firstly, it considers the current state of the plant-based market in Denmark. 
Secondly, it builds a Hidden Markov Model using panel data to explore whether behavioural patterns exist within household’s purchasing of plant-based products.
This model analyses patterns across the categories of dairy, meat, ready meals, and confectionery. The study considers whether there is a likely pattern of adoption for plant-based products at category level.
Results indicate that households in general moved towards a broader plant-based profile, buying products across a wider range of categories through the years of 2018 - 2021. Consumers seem most willing to make the switch to alternative dairy products and least willing to adopt ready meals. This study brings new insights to the plant-based industry and suggests that non-vegetarian households may be coming round to the idea of a diet with more plant-based products.


This repository contains the code used to build the the hidden markov model. These models are especially good to use when you have a set of sequancial observations and believe there may be a latent process driving the patterns you observe. 
Here, the sequential set of observations consists of panel data from 1000 danish households shopping patterns, collected over the four year period from 2018 - 2021.
The data is categorised into 6 types of plant-based products and the final model is run on 4 of these.

The project is split across 4 scripts: pre-processing, categorising the products, coding the product categories, and running the hidden markov model. These can be found in the src folder with comments which outline each step taken within. 

## Repository Folders

The repository has been split into the following folder structure: 

```
 Folder Name                | Purpose                 
 -------------------------- | --------------------  
 data                       | Folder containing the coded data frame 
 plots                      | Folder containing plots and graphs relevant to the study
 output                     | Folder containing tables of the model output 
 src                        | Folder containing the 4 scripts                
 supplementary material     | Folder containing information and descriptions of the panel data used                  
```
