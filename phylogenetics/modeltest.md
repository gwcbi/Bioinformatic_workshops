# Selecting a model of evolution using modeltest-NG
Objective: find out which nucleotide substitution model fits the data the best

## What are models of nucleotide substitution?
A British statistician once wrote: "All models are wrong, some are useful". For each method of tree estimation, you must select a model which the method will use to predict which changes and patterns are more likely given your data. Although no model can fit your data exactly, models can help make predictions about data. The simplest DNA substitution model, JC69, assumes equal base frequencies (25% for each nucleotide) and equal substitution rates for all bases. The most complex model, GTR, allows for 6 different substitution rates for the different nucleotides and 4 different base frequencies (8 free parameters). For an explanation of the common substitution models, see [this helpful guide](http://www.iqtree.org/doc/Substitution-Models).

### Rate heterogeneity across sites
Adding the +I parameter will allow for a proportion of invariable sites. Adding the +G parameter assumes a discrete Gamma model with default 4 rate categories for the sites.

Models can also account for non-stationarity (when your base composition differs accross different lineages of the tree) and non-homogeneity (when your rates vary accross the tree). Actually can they? I'm not sure.

## How to decide which model is best?
We can use likelihood ratio tests (LRTs) or information criterion (BIC, AIC or AICc) to test for which model is the best fit for your data.

## Which model selection tool should I use?
Popular tools jModeltest and ProtTest have been reimplemented as ModelTest-NG, which we will introduce here. IQ-TREE also has a popular model selection feature called ModelFinder known for its algorithmic and computational efficiency, and SMS was recently released which uses heuristic strategies to avoid evaluating the ful set of candidate models.   
