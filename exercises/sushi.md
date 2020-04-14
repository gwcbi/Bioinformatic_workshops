# Lab 1: Suspicious Sushi

## Background
You and some friends have just had a dinner at a local sushi bar. Being the inquisitive biologist, you wonder if your group really ate what was listed on the menu (i.e., was the sashimi really what it claimed to be). So you set out to test this hypothesis by saving a bit of tissue from your sashimi. The menu lists the following possibilities: “Hirame” (flounder), “Sake” (salmon), “Hamachi” (yellowtail), and “Maguro” (tuna) sashimi plates. You ordered the Maguro. Given the following sequence from your dinner, design PCR primers to amplify the following exact sequence of DNA (for the sake of simplicity) from your samples. Assume you collected the following sequence using your PCR primers. Compare this sequence to potential candidate species (for example, what is the relative percent identity of your query sequence to the different target sequences?). Tell me your findings. 
### Your Sequencing Result
This sequence is also provided to you in a file called `sushi.fasta` for your convenience.
```
GCCTTAAGCCTACTCATCCGAGCTGAGCTTAGCCAACCTGGGGCGCTCTTAGGAGACGACCAGATT
TACAATGTTATTGTTACAGCACATGCCTTTGTAATAATTTTCTTTATAGTAATACCAATTATGATC
GGTGGTTTTGGGAACTGACTTGTTCCCTTAATGATTGGAGCTCCTGATATAGCATTTCCTCGAATA
AATAATATGAGCTTTTGACTCCTCCCCCCTTCATTCCTTCTCCTCCTTTCCTCCTCCGGAGTTGAA
GCAGGGGCCGGAACAGGATGAACAGTTTACCCGCCCCTCGCAGGAAACCTCGCCCACGCAGGGGCC
TCCGTAGACCTAACCATCTTCTCCTTACATCTGGCAGGTGTTTCCTCAATTCTGGGGGCCATTAAC
TTCATTACAACCATTATTAATATGAAGCCTCCAGCCATTTCCCAGTATCAAACCCCCCTCTTCGTA
TGATCCGTTTTAATTACAGCAGTCCTCCTCCTTCTATCCCTCCCCGTCCTTGCAGCCGGCATCACC
ATGCTCCTTACAGACCGAAACCTAAATACAACCTTCTTTGACCCCGCAGGAGGAGGAGACCCCATT
TTATACCAACACCTGTTCTGATTCTTTGGCCACCCC
````


0. Using [NCBI BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastSearch), perform a [blast](../phylogenetics/blast.md) search to find out what the closest match to this sequence is. What is the species name? What gene was amplified? How close of a match was it?
1. What are the species names of the fish on the menu? For each of the 4 species, use NCBI to find and download the same gene for each species. Choose two other types of fish, look up their species names, and download the same gene for these species.
2. Use [mafft](../phylogenetics/align.md) to make an alignment of the 7 sequences. What was the length of the original sequences? How many base pairs long is the alignment?
3. Using [RAxML](../phylogenetics/phylogeny.md), make a tree to represent the relationships between the 7 fish species. 
4. View your tree using [Figtree](figtree.md). Which fish species is most closely related to the fish you sequenced from the sushi bar?

***
See the [original article](https://peerj.com/articles/3234/?utm_source=TrendMD&utm_campaign=PeerJ_TrendMD_1&utm_medium=TrendMD)
