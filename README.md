# CASA0012 Dissertation

**Title: Spatial Pattern Mining of Tech Clusters of Dynamics and Industry Mix Based on Quantitative Methods in England Area, UK**

![intro_picture](https://github.com/fang-zeqiang/CASA0012-Dissertation/blob/main/bookdown/general_images/G_enR_v1.png?raw=true)

This repo is to store my dissertation file and present my disseration book

```
|_ bookdown                   # the path of dissertation book
|_ code                       # the path of the reproducible analysis and map making
  |_ sql                      # the folder contains sql scripts for data aggregation
  |_ geoda                    # the spatial pattern EDA project folder
|_ jupyterlab                 # the path of research progress log
|_ dataset                    # the path of data source
|_ CASA0012-Dissertation.pdf  # the paper version of dissertation
```
## Reproducible Analysis Process

|Name|Link|
|:--|:--|
|Exploratory Data Analysis|	https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/EDA.html|
|Descriptive Analysis for Dynamics|https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Dynamics-Research.html|
|Regression Analysis(Top 10 TTWAs)|https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Regression-Research.html|
|Regression Results(All TTWAs)|https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Regression-Results.html|
|Spatial Pattern Research|https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Spatial-Research.html|
|Map Making in R (Distribution)|https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Map-Making-R-dis.html|
|Map Making in R (Morans I and LISA)|	https://rpubs.com/fangzq/UK_ttwa_tmap_making|

## Dataset

|Name|Link|
|:--|:--|
|Dissertation Book Live Version|https://zeqiang.fun/CASA0012-Dissertation/bookdown/html/|
|Data Source Repository|https://github.com/fang-zeqiang/Master-Dissertation/tree/main/Dataset|
|UK Registered Firms|	https://opencorporates.com/info/our-data/|
|Science and Technology Classification|	https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/science-and-technology-classification.xls|
|Travel to Work Area Boundaries|https://github.com/fang-zeqiang/Master-Dissertation/tree/main/Dataset/Travel_to_Work_Areas_2011_guidance_and_information_V5|
|Regression Data|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/df_hh_EnR_ttwaName_asset_not_drop.csv|
|TTWAs with Three Indicators in 1998|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/Spatial/dfm_1998_output.geojson|
|TTWAs with Three Indicators in 2008|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/Spatial/dfm_2008_output.geojson|
|TTWAs with Three Indicators in 2018|https://github.com/fang-zeqiang/Master-Dissertation/blob/main/Dataset/Spatial/dfm_2018_output.geojson|

## Research Progress

1. For very beginning exploratory analysis of `fame_OC.dta`, you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/EDA.html)
1. For further descriptive analysis(dynamics), you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Dynamics-Research.html)
1. For regression analysis, you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Regression-Research.html)(For regression **dataset**, you can access [this page](https://zeqiang.fun/CASA0012-Dissertation/dataset/Top_10_Tech_TTWA_Cluster_Reg_Prepare.xlsx))
2. For [Spatial Research](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/Spatial-Research.html)

## The Cheatsheet

1. The python regression cheatsheet is in this [link](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/example/DSSS_SDC_2021_Workshop_6_Advanced_Regression.html)
1. The python cluster cheatsheet is in this [link](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/example/clustering_workshop_2020.html)
1. The python regression analysis context is in this [link](https://zeqiang.fun/CASA0012-Dissertation/jupyterlab/example/regression_child_poverty.html)

## Feedback

Title:Spatial Pattern Mining of Tech Clusterins of Dynamics and Industry Mix First marker comments per criterion, Review and research framing: 

Chapter 1 has two clear and well-signalled research questions, and a very clear oveview of the the dissertation's objectives and structure. The research questions are well-contextualised, placing the study in the context of tech cluster presence, dynamics and policy concerns in the UK and elsewhere. This chapter draws on a good range of UK sources, not just the obvious Silicon Valley case. This chapter could be clearer on motivation - why do we want to know about *entry* specifically, as opposed to broader questions of firm / cluster performance? The tech clusters literature is very large and thus challenging to summarise. 

Chapter 2 is a compact review which does a good job of picking out the research question-relevant themes [clusters, industrial dynamics, concentration] and linking them back to the research questions / specific empirical context. Ideally, this chapter would then synthesise the findings to develop specific testable hypotheses for each research question - however, that is a big ask of a masters thesis.

Overall, the range of references is impressive, both here and in Chapter 3, although more use could have been made of existing lit reviews / overviews, which give you more 'leverage' over what's known - afaik only Kerr and Robert-Nicoud 2020 is deployed. 

**Research design:** Overall, the research design is original, and demonstrates good understanding of the data and core concepts, as well as critical reflection on their limitations. Core metrics [entry rate, HHI] are carefully explained, although not always correctly notated [e.g. where is _k in the HHI equation on p16; the main estimating equation on p17 needs `_i` and `_t` suffixes, and terms x3 and x4 are missing]. The discussion of the HHI could be clearer - it is a measure of industrial concentration in the sense of measuring the dominance [in firm counts] of any one tech SIC over the others. Given that firms in different SICs may not compete with each other, I'm not sure you can read off competition / market power from this metric. The justification of spatial units is especially clear and thoughtful (this would also be the point to flag that you will look at clustering *across* TTWAs too). However, this material should mention the registered address / true location issue, and be clear that using TTWAs is a workaround for this. The temporal cutoff is well-chosen, though thesis should explain that Companies House drops observations 20 years after company dissolution. 

So given the extraction date (September 2018) it is not surprising #obs is much lower before 2000 than after it. The lagged extraction date may also help explain why dissolution rates are so low (most startups fail after about ~ 3 years). The design is fully reproducible. Data sources and python / r notebooks are easily accessible online. There is also extensive, critical ethical reflection. Raw data is public, collected and cleaned by Open Corporates; care is taken not to disclose individual company names / variables. 

**Analysis and critical reflection:** In Chapter 4, the descriptive analysis is well laid out, with a good balance of visualisation and text, and the main findings are clearly explained. It comes slightly unstuck when discussing trends in the HHI; as above, as built this measures the *internal structure* of the tech industry rather than market competition / concentration, as you end up saying on p26. It is also plausible that the highest %-point increases in entry rates reflect lowest initial stocks - in rural areas like Bridport and Minehead, for example? The regression analysis confirms the descriptive story in Figure 4.1, showing a big positive link from density to entry rates, and a very large negative link from HHI to entry rates. The model fit is a little better once London is taken out, but coefficients are broadly similar. 

This section would benefit from some discussion about why that is. In terms of telling your story, I think Table 4.3 should probably come before 4.2. 4.3 is doing stepwise analysis, showing us that your full model has additional explanatory power; 4.2 is showing us how the story changes when you include / exclude London. More broadly, this part would benefit from thinking about why there is a such a strong link from density to entry rate. Could at least some of this be mechanical, since in Figure 4.1 the two measures move very closely together? Similarly, there is a strong inverse relationship in the time series for entry rates and HHI. Lagging HHI and density in your regressions would help resolve this. It would also benefit from estimating a model with additional time-varying controls e.g. population density, % graduates in the workforce, firm age structure. 

From other studies in the literature, we know that these factors are linked to firm entry rates. There is a risk your model is picking up these factors in the HHI / density coefficients. Ch 5 has a concise summary of results are shows evidence of extensive critical reflection, linking results to wider UK policy discussion and (to some extent) to the existing literature reviewed in Chapter 2. There is also a note on limitations, some high-level recommendations for policymakers and some suggestions for future work. 

**Visualisation and communication:** Overall, visualiation and communication is exemplary. The thesis' language is mostly punchy and clear. Formulae are carefully explained. Graphs and maps are appropriate for the content, clear and easy to read. Descriptive and results tables are clearly formulated, with proper publication-style reporting of regression results. Helpfully, chapters / subsections and online content are all hyperlinked. 

The caveats are: 
  
  1) in some descriptive tables [e.g. 4.1], we don't need to see results to multiple decimal places, 2-3 would do; 
  2) there are multiple typos / instances of missing text, e.g. p5 [They], p6 [clutser], p9 [etc], p10 [is, attribute, time and], p13 [floating sentence]. A further copy-edit would clean these up; 
  3) formulae are not always fully/correctly notated. Minor point - for your loglinear models, it would be helpful to transform the exponentiated b's into real numbers. E.g. in model 2, a one-unit change in cluster density is linked to ~39% increase in cluster entry rate. General comments (optional): Second marker comments: I had trouble making sense of many of the metrics used: they were not clearly explained and it was often impossible to tell whether their construction was appropriate to the data (since the extraction/aggregation process wasn't clearly expleined either). 

This makes it hard to interpret the finding that, for instance, 'tech clustering' is higher in areas we don't associate with tech (I think it's the way the HHI was used with no minimum threshold) and it is only, for instance, mentioned in passing that London was excluded from the analysis! There was no attempt to incorporate the type of industry, so Cambridge 'tech cluster' is very different from Reading/Slough/Maidenhead corridor, which is different againt from Bristol... I have a really hard time knowing if any of these results are meaningful: the entire analysis proceeds *as if* the data are 'correct' and the results as well. There's no validation or attempts to connect the results to 'pen portraits' or other evdience (e.g. the literature!) of different areas. I may be being a bit harsh here.

<!--
## Reference

0. We have not done a lot to interpret the models. If you have time and energy, here is a handy book on interpretation of statistics and machine learning models. For linear regression, please read this [this chapter](https://christophm.github.io/interpretable-ml-book/limo.html). For decision trees, have a look at [this chapter](https://christophm.github.io/interpretable-ml-book/tree.html). If you want to interpret a random forest, you can try the **permutation feature importance** method, which is introduced in [this chapter](https://christophm.github.io/interpretable-ml-book/feature-importance.html).
1. We committed a methodological sin in reusing the same dataset for model fitting and validation (calculting the goodness-of-fit). There are ways around this problem, either by using another dataset, or by splitting the dataset into parts for *cross-validation*. Look at the documentation on cross-validation [here](ttp://scikit-learn.org/stable/modules/cross_validation.html)and then implement a simple technique to avoid this problem.
2. There are lots of nice datasets for analysis on [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets.html) and [Kaggle](https://www.kaggle.com/datasets). Take a look, and if any of them take your fancy try create a regression model. Which data features are important? Which are not? 
-->
