# VIS Evaluation Analysis
Analysis of features and trends from evaluation practices described in IEEE VIS application papers from 2018 to 2022.

Authors: Yiwen Xing, Gabriel D. Cantareira, Rita Borgo, and Alfie Abdul-Rahman.

## How to use this repository

This repository contains a .csv file with basic information from several IEEE VIS papers (e.g., title, authors, year) and coding information from assigning their evaluation practices different categorical or quantitative properties (e.g., evaluation goals and methods, number of participants, stage of development). This data file also has a few papers with multiple rows, representing papers that contain multiple evaluation steps.

This repository also contains a Python notebook with code for conducting certain statistical analysis on this data as described in our research paper, "A Comprehensive Analysis of Evaluation Practices in VIS Domain Applications".

To run this code, we recommend a Python notebook environment running Python 3.12.

The versions of required libraries used to run the analysis in the paper are as follows:

```
numpy v1.22.4
pandas v2.0.3
matplotlib v3.7.3
seaborn v0.13.0
mlxtend v0.23.0
networkx v3.1
statsmodels v0.14.0
```


## Paper Selection

Our aim was to conduct analysis on the evaluation practices of IEEE VIS domain application papers. While the VIS conference does have a distinct category for application research, this classification primarily guides authors during submission and does not facilitate direct retrieval of papers under an “Application” category from published works. We therefore consulted the VIS Area Models and drew inspiration from topics listed under “Application” type, including “Application Domains”, “Application-specific Technical Solutions”, and “Insight Documentation” to make a selection of papers to examine. 

We obtained information from all IEEE VIS papers from the years 2018-2022 (IEEE TVCG special issues on IEEE VIS), consisting of a total of 620 papers (2018: 120, 2019: 120, 2020: 150, 2021: 110, 2022: 120). Our process consisted of an automated filtering to detect keywords related to application-focused research, domain user involvement, and evaluation practices, resulting in a list of 303 papers that are contained in the .csv file in this repository. 

This step was followed by two rounds of manual filtering to identify papers focused on applications or that offered domain application case studies. The column "Final Check" in the data indicates this manual filtering: we assigned 1 for papers kept in the selection, 0 or 999 for papers dropped. The end result was a curated list of 140 papers involving domain applications.

