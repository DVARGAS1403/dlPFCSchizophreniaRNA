# dlPFCSchizophreniaRNA
Code for replicating analyses of:

"DLPFC Transcriptome Defines Two Molecular Subtypes of Schizophrenia"

Elijah F W Bowen  
Jack L Burgess  
Richard Granger  
Joel E Kleinman  
C Harker Rhodes

## Installation
Once the below requirements are installed, the code will run without any build/compilation steps. You may check out this repository or simply download a zip. Please watch for new commits.

## Requirements
* R (validated to run on versions 3.3.2 linux and 3.4.3 windows)
* RStudio (highly recommended since code are .Rmd markdown files, not .R scripts)
* R CRAN packages:
    * robust
    * robustlmm
    * WGCNA
    * igraph
    * statmod
    * stringr
* Certain scripts also require BioConductor packages, which are best installed from the BioConductor folks:
    * beadarray
    * edgeR
    * GenomicFeatures
    * lumi
    * illuminaHumanv4.db

## Data
This code runs on data which is access-controlled by third parties (dbGaP study accession phs000979.v1.p1, CommonMind Consortium http://www.synapse.org/cmc). We cannot redistribute the data, but feel free to email us with questions.

## Description of code
Scripts are numbered in a reasonable sequential order.

* NIH dataset
    * Pre-processing
        * 1
        * 2
        * 3
    * Analyses
        * 4
        * 5
        * 6
* CMC dataset  
    * Pre-processing
        * 8a
    * Analyses
        * 8b
        * 8c
        * 8d
