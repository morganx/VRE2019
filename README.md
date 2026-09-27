# VRE2019

This repository contains source code and supporting material for the manuscript:
"Agricultural origins of a highly-persistent lineage of vancomycin-resistant Enterococcus faecalis in New Zealand" 

Rowena Rushton-Green, Rachel L Darnell , George Taiaroa, Glen P Carter, Gregory M Cook, Xochitl C Morgan

This manuscript is published in [Applied & Environmental Microbiology](https://aem.asm.org/content/85/13/e00137-19) ([PubMed](https://pubmed.ncbi.nlm.nih.gov/31028029/)). All assemblies are available at NCBI's Sequencing Read Archive (BioProject: PRJNA476469)

> **GitHub mirror note:** This repository was originally published in GitLab. This repository contains the complete code and supporting material from the original project except for five generated Gubbins outputs that exceed GitHub's 100 MB per-file limit. The intact archival repository, including those files and the original Git history, remains available on [GitLab](https://gitlab.com/morganx/vre2019).

## Oversized generated files retained on GitLab

The following derived analysis files are intentionally omitted from the GitHub mirror. They can be viewed or downloaded from the archival GitLab repository:

- [`data/Gubbins/Faecium/all_faecium/all_faecium.branch_base_reconstruction.embl`](https://gitlab.com/morganx/vre2019/-/blob/master/data/Gubbins/Faecium/all_faecium/all_faecium.branch_base_reconstruction.embl)
- [`data/Gubbins/Faecalis/All_Strains/all_faecalis.fa.gz`](https://gitlab.com/morganx/vre2019/-/blob/master/data/Gubbins/Faecalis/All_Strains/all_faecalis.fa.gz)
- [`data/Gubbins/Faecium/all_faecium/all_faecium.fa.gz`](https://gitlab.com/morganx/vre2019/-/blob/master/data/Gubbins/Faecium/all_faecium/all_faecium.fa.gz)
- [`data/Gubbins/Faecium/faecium_no_outliers/all.branch_base_reconstruction.embl`](https://gitlab.com/morganx/vre2019/-/blob/master/data/Gubbins/Faecium/faecium_no_outliers/all.branch_base_reconstruction.embl)
- [`data/Gubbins/Faecium/faecium_no_outliers/all.fa.gz`](https://gitlab.com/morganx/vre2019/-/blob/master/data/Gubbins/Faecium/faecium_no_outliers/all.fa.gz)


## Analysis notes

-The R code in Ro-FIgures.RMD contains code to make Figures 1-3 and Supplementary Figures 2-6 and 8-11.  

-The values for Figure 4 are derived from averages of data provided in Supplementary Table 8 (bp distance between antibiotic resistance genes, average contig length containing multiple antibiotic resistance genes, number and percentage of isolates in subset containing multiple antibiotic resistance genes)

-Supplementary Figure 6 produced from visualisation of Illumina-corrected PacBio sequenced plasmids of AR01/DG in Geneious
 
-The nullarbor execute command to produce a make file in an output directory (square brackets indicate variable inputs):
perl /APPS/linuxbrew/bin/nullarbor.pl --name [NAME] --mlst [efaecium OR efaecalis]  --accurate --ref [REFERENCE.FASTA] --input [INPUT TAB FILE] --outdir [OUTPUT DIRECTORY]

-To run make file:
cd [OUTDIR]
nohup make -j 4
