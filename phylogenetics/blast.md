# Understanding DNA sequences and using BLAST and NCBI

## How are DNA sequences represented?
DNA sequences are usually represented in fasta or fastq format. Here is an example of a DNA sequence in FASTA format:
```
>HQ986301.1 
AACACTTTATTTTTTATTTGGAGCATGATCAGGGATGGTAGGAACTGCTCTAAGAGTCCTAATTCGAATT
GAATTAGGACAACCAGGATCATTAATTGGAGATGATCAAATTTATAATGTAATTGTAACAGCTCATGCTT
TTGTTATAATTTTCTTTATAGTAATACCTATTATAATTGGAGGATTTGGAAATTGATTAGTGCCACTAAT
ATTAGGAGCACCTGATATAGCTTTCCCACGATTAAATAATATAAGATTTTGATTATTACCACCTTCTCTT
ACACTTTTATTAGCAGGAAGTATAGTTGAAAGAGGTGCAGGAACAGGATGAACAGTTTATCCTCCTCTTG
CTGGTGCTATTGCTCATGCAGGAGCATCTGTAGATTTAACTATTTTTTCCCTTCACTTAGCTGGTGTATC
TTCAATTTTAGGTGCTATTAATTTTATTACTACAACAATTAATATAAAGTCACCAGGGATAAAGATAGAT
CAAATACCATTATTTGTATGAGCCGTAGTAATTACAGCTGTATTATTATTATTATCTCTTCCTGTTCTTG
CTGGTGCAATTACAATATTATTAACAGATCGAAATATTAATACATCATTCTTTGATCCTGCAGGAGGGGG
TGATCCAATTCTTTATCAACATTTATTT
```
As you can see, the first line begins with a `>` and gives a string of numbers and some descriptive words. The second line gives a series of A's, T's, C's and G's. This doesn't tell us much about what kind of dna it is, or where it is from. We can look this up using BLAST.

When you generate your own sequences using illumina, sequences are often in fastq format. This means that there are quality scores that are important for assembly.

## How do you find the closest match to a DNA sequence using BLAST?
### What is BLAST?
BLAST stands for Basic Local Alignment Search Tool. BLAST allows you to query the NCBI database to find similar sequences.
0. Copy the sequence above and paste into the [BLAST browser](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PAGE_TYPE=BlastSearch).
1. Scroll down to the bottom of the page and click the blue `BLAST` button. You can change the settings, but for our case, the default settings work well.
2. After a few minutes, you should get an output similar to below. The first line gives the description of the closest match to your sequence. In the second to last column, you can see the percent identity. In this case, the first sequence listed here is 100% similar to our sequence.<br/>
![BLAST1](images/BLAST1.png)
3. Click on the accession number, listed in the last column. Here you can see much more information. What gene is this from? What other information can you see?
![BLAST2](images/BLAST2.png)
4. To download the sequence, click on the fasta button on the top left. Then click `send to` then `file` then set the format as `fasta`.
![BLAST3](images/BLAST3.png)

*For more information about using BLAST, see the [BLAST topic page](https://blast.ncbi.nlm.nih.gov/Blast.cgi?CMD=Web&PAGE_TYPE=BlastDocs&DOC_TYPE=BlastHelp)*
## How do I search for a specific sequence or gene using NCBI?
