README

This repository contains source code and supporting material for the manuscript:

Agricultural origins of a highly-persistent lineage of vancomycin-resistant Enterococcus faecalis in New Zealand 

Rowena Rushton-Green, Rachel L Darnell , George Taiaroa, Glen P Carter, Gregory M Cook, Xochitl C Morgan

This manuscript is published at Applied & Environmental Microbiology:
https://aem.asm.org/content/85/13/e00137-19


Notes:

-The R code in Ro-FIgures.RMD contains code to make Figures 1-3 and Supplementary Figures 2-6 and 8-11.  

-The values for Figure 4 are derived from averages of data provided in Supplementary Table 8 (bp distance between antibiotic resistance genes, average contig length containing multiple antibiotic resistance genes, number and percentage of isolates in subset containing multiple antibiotic resistance genes)

-Supplementary Figure 6 produced from visualisation of Illumina-corrected PacBio sequenced plasmids of AR01/DG in Geneious
 
-The nullarbor execute command to produce a make file in an output directory (square brackets indicate variable inputs):
perl /APPS/linuxbrew/bin/nullarbor.pl --name [NAME] --mlst [efaecium OR efaecalis]  --accurate --ref [REFERENCE.FASTA] --input [INPUT TAB FILE] --outdir [OUTPUT DIRECTORY]

-To run make file:
cd [OUTDIR]
nohup make -j 4
