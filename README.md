# Introduction 
Cluster randomized trials are randomized controlled trials where individuals are randomly assigned into groups called clusters. This paper presents a collaborative effort with Dr. Zhijin Wu from the Biostatistics Department at Brown University to address a fundamental challenge in experimental design: how to allocate resources optimally under budget constraints to maximize the precision of treatment effect estimation.We will consider a cluster randomized trial in which we will assign observations to either the control or treatment group and our goal is to estimate the treatment effect on an outcome variable Y.

Our focus is on designing a simulation study to investigate optimal experimental design strategies for cluster randomized trials under budget constraints. More specifically, we aim to determine the ideal allocation of resources between the number of clusters and the number of observations within each cluster, given a fixed budget \( B \). While we consider \( B \) in monetary terms, a key feature of our framework is the cost structure: the initial sample from a cluster incurs a higher cost (\( c_1 \)), while subsequent samples within the same cluster are relatively cheaper (\( c_2 < c_1 \)). 

An additional consideration in our design is the inherent correlation among samples within the same cluster. While increasing the number of observations per cluster can reduce costs, the correlated nature of these observations may diminish their marginal contribution to the precision of treatment effect estimation. In other words,  while samples from the same cluster are cheaper , samples within a cluster may be correlated. In consideration of sequencing data, samples within a cluster might correspond to collecting technical replicates(repeated measurements) and different clusters correspond to biological replicates(measurements from different samples).Technical replicates are cheaper to obtain but are highly correlated.Our simulation study will explore this tradeoff and provide insights into the optimal balance between cluster size and cluster number, with the goal of maximizing efficiency while adhering to resource constraints.  

In this study, we will focus on three aims:
*Aim 1*: Design a simulation study using the ADEMP framework from class to evaluate potential study designs,
*Aim 2*: Explore relationships between the underlying data generation mechanism parameters and the relative costs  (\( c_2 /c_1 \)) and how these impact the optimal study design.
*Aim 3*: Extend your simulation study to the setting in which Y follows a Poisson distribution with mean $\mu_i$\ and explore how this impacts the results. The hierarchical model for this setting is given below.

By leveraging simulation-based methods, we aim to contribute to the development of cost-effective and statistically rigorous approaches for designing cluster randomized trials.  


