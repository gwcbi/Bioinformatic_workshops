# Volcano Plots
![volcano plot](./Images/VolcanoPlot.png)


Volcano plots are used to visualize the results of differential gene expression analysis.

In this module, we will construct a volcano plot for real data generated from an RNA-seq analysis of Systemic Lupus Erythematosus.

Dots in a volcano plot typically represent genes, a volcano plot's y-axis indicates the -log(p-value) and the x-axis indicates the log fold change in expression value. As such, dots in the upper right of the plot indicate genes with high, positive log fold change values which are very statistically significant (low p-value).

We will create our volcano plot in RStudio.

Open RStudio and create a new R Script by clicking File->New File->R Script

Save the file as "VolcanoPlot.R" and Session->Set Working Directory->To Source File Location

Make sure you have the differential expression data (AllDifferentiallyExpressed.csv) in the same directory.

We will load our libraries first:

```
library(ggplot2)
```

Next we will load our data

```
genes <- read.csv(file="AllDifferentiallyExpressed.csv", header=TRUE, sep=",")
```

We will identify the upregulated and downregulated genes:
