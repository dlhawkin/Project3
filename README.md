![Hospitals](https://github.com/user-attachments/assets/66c4d062-bccb-4b83-90db-b98d3925b244)
# Budget Constraints using Simulated Data
# Introduction 
Cluster randomized trials are randomized controlled trials where individuals are randomly assigned into groups called clusters. This paper presents a collaborative effort with Dr. Zhijin Wu from the Biostatistics Department at Brown University to address a fundamental challenge in experimental design: how to allocate resources optimally under budget constraints to maximize the precision of treatment effect estimation.We will consider a cluster randomized trial in which we will assign observations to either the control or treatment group and our goal is to estimate the treatment effect on an outcome variable Y.

Our focus is on designing a simulation study to investigate optimal experimental design strategies for cluster randomized trials under budget constraints. More specifically, we aim to determine the ideal allocation of resources between the number of clusters and the number of observations within each cluster, given a fixed budget \( B \). While we consider \( B \) in monetary terms, a key feature of our framework is the cost structure: the initial sample from a cluster incurs a higher cost (\( c_1 \)), while subsequent samples within the same cluster are
 relatively cheaper (\( c_2 < c_1 \)). 

An additional consideration in our design is the inherent correlation among samples within the same cluster. While increasing the number of observations per cluster can reduce costs, the correlated nature of these observations may diminish their marginal contribution to the precision of treatment effect estimation. In other words,  while samples from the same cluster are cheaper , samples within a cluster may be correlated. In consideration of sequencing data, samples within a cluster might correspond to collecting technical replicates(repeated measurements) and different clusters correspond to biological replicates(measurements from different samples).Technical replicates are cheaper to obtain but are highly correlated.Our simulation study will explore this tradeoff and provide insights into the optimal balance between cluster size and cluster number, with the goal of maximizing efficiency while adhering to resource constraints.  

In this study, we will focus on three aims:
*Aim 1*: Design a simulation study using the ADEMP framework from class to evaluate potential study designs,
*Aim 2*: Explore relationships between the underlying data generation mechanism parameters and the relative costs  (\( c_2 /c_1 \)) and how these impact the optimal study design.
*Aim 3*: Extend your simulation study to the setting in which Y follows a Poisson distribution with mean $\mu_i$\ and explore how this impacts the results. The hierarchical model for this setting is given below.



# Data
This study consists on simulated data (1000) with varied gammas, sigmas, c1 representing costs, and c2 representing additional costs.
# Key Files
`Project3Simulation.pdf`: Finalize report that consist of budget constraint analysis using simulation modeling.  `Project3Simulation.Rmd` : Rmd file that contains code, analysis and interpretations.



  # Dependencies
The R version and poackages used in this project are indicated below: `R version 4.2.3 (2023-03-15)`

`magick_2.8.5`
`ggwordcloud_0.6.2`
`reshape2_1.4.4`
`corrplot_0.94`
`mice_3.16.0`
`gt_0.11.1`
`gtsummary_2.0.2` 
`visdat_0.6.0`   
`naniar_1.1.0`
`GGally_2.2.1`
`knitr_1.46`
`kableExtra_1.4.0`
`MASS_7.3-58.2`
`lubridate_1.9.3`
`forcats_1.0.0` 
`stringr_1.5.1` ,   
`dplyr_1.1.4`
`purrr_1.0.2`
`tidyr_1.3.1` 
`tibble_3.2.1`,  
`ggplot2_3.5.1` 
`tidyverse_2.0.0 ` 
`readr_2.1.5`  
