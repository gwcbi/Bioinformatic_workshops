# Understanding the phylogenetics and evolution of COVID-19

The purpose of this exercise is to get an overall picture of the evolution of this group and estimate the ancestral sequences for
1) The COVID-19 clade MRCA, 
2) The (at least) two SARS MRCAs just after the zoonoses from bats, 
3) The overall SARS MRCA, and 
4) The SARS + MERS MRCA.

As such, the tasks here are:

1) download the sequences in fasta format and merge the NCBI+GISAID data.
2) search for duplicates and quantify the overlap between the two databases.
3) align with MAFFT
4) use ModelTest-NG within RAxML to get a best-fit model
5) estimate an ML tree with RAxML with at least 10 random additions. 
6) The best RAxML tree has to be uploaded in FigTree to be rerooted and then reloaded in RAxML to estimate ancestral sequences via marginal ancestral stat reconstruction
7) with the rooted tree, you can get ML marginal ancestral state reconstructions for the nodes of a tree.

