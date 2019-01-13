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
        * 1-Format_phenotype_data.Rmd
        * 2-Format_idat_files.Rmd
        * 3-Filter_dlpfc_array_data.Rmd
    * Analyses
        * 4-Sz_cohort_demographics.Rmd
        * 5-Robust_lmer.Rmd
        * 6a-Cluster_schizophrenics.Rmd
        * 6b-Perturbation_stability_of_clustering.Rmd
        * 6c-Antipsychotics.Rmd
        * 6c-Subgroup_demographics.Rmd
        * 6d-Graphical_analysis.Rmd
        * 7a-Robust_lmer_with_sz_subtype_1.Rmd
        * 7b-Robust_lmer_with_sz_subtype_2.Rmd
        * 7-Figures_and_tables.Rmd
        * 7-Figures_and_table_from_residuals.Rmd NOT USED IN MANUSCRIPT
        * 7-Comparing_hit_lists.Rmd NOT USED IN MANUSCRIPT
* CMC dataset  
    * Pre-processing
        * 8a-Preprocess_cmc_data.Rmd
    * Analyses
        * 8b-CMC_cohort_demographics.Rmd
        * 8c-Pitt_cohort_de_analysis.Rmd
        * 8d-Clustering_of_pitt_cohort_schizophrenics
