##### Rationale

Estimating speciation and extinction rates is fundamental to understanding the processes that have shaped biodiversity over time and how life may respond to environmental catastrophe in the near future. >99% of life that has ever existed is now extinct and so most of the information we have about the history of life comes from the fossil record. However, the fossil record is a very incomplete record of life, and so reconstructing evolutionary dynamics in deep time requires a modeling approach that explicitly acknowledges unknowns and uncertainties.

![tree](data/projects/images/tree.png)

##### Approach

We have developed a set of mathematical models (the fossilized birth-death process) that can be used to estimate speciation and extinction rates, while accounting for several sources of uncertainty. The model reconstructs evolutionary dynamics (the tree structure shown above in black) from fossils (the orange circles) that are sampled from geological intervals. The current implementation of the model is written C++ in the phylogenetic software package DPPDiv: [https://github.com/trayc7/FDPPDIV](https://github.com/trayc7/FDPPDIV).

##### Challenges

Since our goal is to understand processes operating over very long time periods (10 – 100s myr), the model requires large datasets, containing 1000s of fossil species. This makes the calculation of the likelihood function computationally demanding. In particular, the way we handle uncertainty in the structure of the tree is currently very time consuming.

- The aim of this project is to implement an efficient algorithm, for the calculation of the likelihood function used to estimate speciation and extinction rates. 

##### Requirements

- This project is ideal for students interested in software development and code optimization problems
- The student should be familiar with or willing to learn C++
