
[![describtor - e.g. python version](https://img.shields.io/badge/R%20Studio-Version%201.4-9cf)](www.desired_reference.com)


# Hidden Markov Modelling: How does the plant based market grow? 
----- 

<div align="center"><img src="https://github.com/Orlz/Hidden_Markov_Modelling/blob/main/supplementary_material/vegan.png"width = 100/></div>

----- 


The plant-based food market has experienced rapid growth over the past five years, with many consumers opting to reduce their meat and dairy consumption under the principle of a more sustainable future. 
This conscious choice has been felt within the food market as an upsurge in demand for plant-based products coupled with a notable increase in government funding into the plant protein industry. 

This 2-fold study looks at how the plant-based food market has evolved in Denmark and how non-vegetarian households have been adopting plant-based products. It builds a Hidden Markov Model using panel data to explore whether behavioural patterns exist within household’s purchasing of plant-based products across the categories of dairy, meat, ready meals, and confectionery. 

The project is split across 4 scripts: pre-processing, categorising the products, coding the product categories, and running the hidden markov model. These can be found in the ```src``` folder with comments which outline each step taken within. 

## Table of Contents 

- [Methodological Description](#Methodological)
- [Repository Structure](#Repository) 
- [Data and Scripts](#Data)
  * [Data](#Data)
  * [Scripts](#Scripts)
- [Summary of Results](#Summary)
- [Contact](#Contact) 


## Methodological Description

The repository here holds the scripts used to refine, clean, and code, the panel data from 1000 danish households shopping patterns. These have been collected over the four year period from 2018 - 2021. A Hidden Markov Model is then built to uncover latent patterns in the sequancial observations. 
This methodological choice was motivated by the belief that a latent process was driving the observed purhases of plant-based products, which a Hidden Markov Model would be able to detect by iteratively classifying households into hidden "states" at each time step based on their purchasing behaviour. Observing the net movement of households between these states would then reveal if latent processes were driving the purchases. 


## Repository Structure

The repository has been split into the following folder structure: 

```
 Folder Name                | Purpose                 
 -------------------------- | --------------------  
 data                       | Folder containing the coded data frame 
 plots                      | Folder containing plots and graphs relevant to the study
 output                     | Folder containing tables of the model output 
 src                        | Folder containing the scripts                
 supplementary material     | Folder containing information and descriptions of the panel data used                  
```

## Data and Scripts

### Data 

The model is based upon consumer panel data collected from market intelligence agency [GFK](https://www.gfk.com/about-gfk). This contains a precise extract of the sales, product, and background information for the grocery purchases of 1000 non-vegetarian Danish households. This data is protected and therefore cannot be uploaded to GitHub, however an anonomysed extract of coded data is included in the ```data``` folder. 

### Scripts 

The project is split across a series of four R scripts: 

```
 Script                       | Function                 
 ---------------------------- | --------------------  
 1_GFK_Preprocessing.Rmd      | Initial merging and cleaning of the raw data files
 2_Categorising_Products.Rmd  | Finding and categorizing plant-based products 
 3_Coding_Cateogries.Rmd      | Matching plant-based sales and coding these for the model
 4_HMM_Model.Rmd              | Modelling the data using a hidden markov model                               
```

## Summary of Results 

The model results indicate that a general increasing trend exists across plant-based purchases, meaning Danish household's are expanding their purchasing patterns of plant-based products into new categories over time. 
The below plot shows the state membership of households across the eight 6-month periods, beginning in January 2018 and ending in December 2021. 
The states are organised such that State 1 is the most 'plant-friendly' state, where households buy products across multiple categories, while State 5 is the least 'plant-friendly' state, where households buy very few plant-based products. 
We see a growth in membership of State 1 and State 2 over time, which appears to be coming predominantly from State 3 and a little from State 5. 
This would suggest that households in the middle are moving from narrow plant-based profiles into more broad profiles, thereby indicating non-vegetarian households are becoming more willing to adopt plant-based products into their weekly shop. This gives hope to environmentalists and governments alike, who are actively nudging society towards a more plant-forward diet. Both for themselves, and for the planet. 

<div align="center"><img src="https://github.com/Orlz/Hidden_Markov_Modelling/blob/main/plots/Marginal_Distribution.png"width = 700/></div>


### Contact 
If you are interested in the insights or methodology behind this project, you are always welcome to reach out to me here on GitHub! :earth_africa: :seedling:
