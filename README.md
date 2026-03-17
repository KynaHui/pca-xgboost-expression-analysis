# Genomic Data Analysis

This repository contains the bioinformatics pipeline and analysis for identifying DNA-binding protein motifs and characterizing genomic variants (SNPs) within a specific dataset. This project was completed as part of the Data Analysis in Biomedical Engineering course at The Chinese University of Hong Kong.

## Objectives
* Identify significant DNA-binding motifs from genomic sequences using computational tools.
* Perform variant calling and annotate Single Nucleotide Polymorphisms (SNPs).
* Analyze the functional impact and distribution of variants within the targeted genomic regions.

## Methodology
The analysis was divided into two major components:

### 1. Motif Recognition and Analysis
* **Tools Used:** MEME Suite (Multiple Em for Motif Elicitation).
* **Process:** Analyzed 20 sequences to identify significant protein-binding motifs.
* **Key Findings:** Identified top-ranking motifs with highly significant E-values (e.g., 2.1e-015), representing strong candidates for DNA-binding protein recognition sites.

### 2. SNP Identification and Characterization
* **Pipeline:** Sequence alignment, variant calling, and annotation.
* **Variant Statistics:**
    * Identified a total of 15 SNPs.
    * **Zygosity:** 80% (12) were heterozygous; 20% (3) were homozygous.
    * **Mutation Type:** 11 transitions (Ts) and 4 transversions (Tv).
    * **Ts/Tv Ratio:** 2.75, which is consistent with the typical expected ratio (~2.0-3.0) for human genomic data, indicating high-quality variant calling.
* **Functional Impact:** Analyzed the distribution of SNPs across genomic features (Exonic, Intronic, Intergenic, UTR) to determine potential functional consequences.

## Tech Stack
* **Languages:** Python / R (for statistical analysis and visualization)
* **Bioinformatics Tools:** MEME Suite, variant calling pipelines (e.g., GATK or BCFtools), and annotation databases.

## How to Run
### Prerequisites
* Python 3.x or R environment.
### Execution
1. **Motif Analysis:** Input the provided FASTA sequences into the MEME tool to replicate the motif discovery results.
2. **Variant Analysis:** Use the provided VCF files or scripts to generate the SNP statistics and Ts/Tv ratio plots.
