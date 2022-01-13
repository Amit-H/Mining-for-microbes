# Mining for Microbes 
## Repurposing whole transcriptome data in the pursuit of microbiome characterisation

> This is a brief summary of my Masters thesis which was completed for the completion of the MSc Biomedical Sciences (Medical Microbiology) at Keele University. The data and techniques presented herin are unpublished and not peer reviewed, and this work received a distinction. The original thesis is over 12 thousand words and cannot be uploaded publically, however, this brief version encompasses the main points, techniques and limitations that were covered. If you have any questions regarding my methodology or results, please feel free to open an issue above!

### Summary of research

Data recycling is a potential solution for using the growing quantity of single use biological data from an  environmental and economic perspective, allowing economies of scale to lower experimental costs when considering cost per use. The abundance of public sequence data could present a novel opportunity to increase understanding of the human microbiome. ***It is hypothesised that by repurposing human whole transcriptome RNA data, non-host RNA reads can potentially reflect the state of the microbiome at time of sampling.***  5 studies containing lung, tongue, cervix, and liver whole transcriptome data was accumulated, resulting in 59 samples from either healthy or cancerous tissue; this was obtained from the NCBI Sequence Read Archive and downloaded to Galaxy Europe for analysis. **Data was parsed through a pipeline consisting of FastQC and MultiQC for quality control, HISAT2 for sequence alignment to the human genome assembly Hg38 and unmapped reads separation, and Kraken2 for taxonomic classification.** The results suggest that Kraken2 is a suitable tool for detecting microbial taxa from non-host reads generated from HISAT2 alignment. The generated cervical microbiome closely matched to current literature, and the characterised lung and tongue microbiomes also correlated with findings in the literature. ***The liver data presented entirely novel findings and characterised the liver microbiome at a previously unreported resolution.*** The results are limited by:
* Large confidence intervals
* The presence of contamination within the samples during sequencing
* A large quantity of human reads remaining post mapping
* Low genomic coverage per species due to coverage bias 
* Data granularity limited to the genus level. 

There is a substantial basis to further test the hypothesis with a wider variety of sample types in the pursuit of data reuse for microbiome characterisation.