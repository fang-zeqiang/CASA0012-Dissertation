# CASA0012-Dissertation

This repo is to store my dissertation file and present my disseration book

```
- bookdown #the path of dissertation book
- jupyterlab #the path of research progress log
- code #the path of the reproducible analysis and map making
```
## Research Progress

1. For very beginning exploratory analysis of `fame_OC.dta`, you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/EDA.html)
1. For further descriptive analysis(dynamics), you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Dynamics-Research.html)
1. For regression analysis, you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Regression-Research.html)(For regression **dataset**, you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/dataset/Top_10_Tech_TTWA_Cluster_Reg_Prepare.xlsx))
2. For [Spatial Research](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Spatial-Research.html)

## Dataset

|Name|Link|
|:--:|:--:|
|Dissertation Book Live Version|https://zeqiang.fun/CASA0012-Dissertation/bookdown/html/|
|Data Source Repository|https://github.com/fang-zeqiang/Master-Dissertation/tree/main/Dataset|
|UK Registered Firms|	https://opencorporates.com/info/our-data/|
|Science and Technology Classification|	https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/science-and-technology-classification.xls|
|Travel to Work Area Boundaries|https://github.com/fang-zeqiang/Master-Dissertation/tree/main/Dataset/Travel_to_Work_Areas_2011_guidance_and_information_V5|
|Regression Data|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/df_hh_EnR_ttwaName_asset_not_drop.csv|
|TTWAs with Three Indicators in 1998|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/Spatial/dfm_1998_output.geojson|
|TTWAs with Three Indicators in 2008|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/Spatial/dfm_2008_output.geojson|
|TTWAs with Three Indicators in 2018|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/Spatial/dfm_2018_output.geojson|

## The Cheatsheet

1. The python regression cheatsheet is in this [link](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/example/DSSS_SDC_2021_Workshop_6_Advanced_Regression.html)
1. The python cluster cheatsheet is in this [link](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/example/clustering_workshop_2020.html)
1. The python regression analysis context is in this [link](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/example/regression_child_poverty.html)

## Reference

0. We have not done a lot to interpret the models. If you have time and energy, here is a handy book on interpretation of statistics and machine learning models. For linear regression, please read this [this chapter](https://christophm.github.io/interpretable-ml-book/limo.html). For decision trees, have a look at [this chapter](https://christophm.github.io/interpretable-ml-book/tree.html). If you want to interpret a random forest, you can try the **permutation feature importance** method, which is introduced in [this chapter](https://christophm.github.io/interpretable-ml-book/feature-importance.html).
1. We committed a methodological sin in reusing the same dataset for model fitting and validation (calculting the goodness-of-fit). There are ways around this problem, either by using another dataset, or by splitting the dataset into parts for *cross-validation*. Look at the documentation on cross-validation [here](ttp://scikit-learn.org/stable/modules/cross_validation.html)and then implement a simple technique to avoid this problem.
2. There are lots of nice datasets for analysis on [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.html) and [Kaggle](https://www.kaggle.com/datasets). Take a look, and if any of them take your fancy try create a regression model. Which data features are important? Which are not? 
