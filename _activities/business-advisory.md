---
title: 'Multi-omics'
image: '/activities/default.png'
---

The Next Generation Sequencing (NGS) produce big biological data including studies of whole genomes (whole-genome sequencing), smaller regions of the genome (exome sequencing), of the transcriptome (RNA-seq), the methylome (Bisulfite-seq) and protein-DNA binding sites (ChIPseq). 
The raw NGS data are consequently analyzed by established and widely accepted bioinformatics tools (bwa, TrimGalore, HISAT2, MACS2, R). The process of analyzing omics data usually leads to a high dimensional matrix, with the different cases listed as columns and the locations on the genome in which the examined event happened (e.g. mutation, gene expression etc.) as rows.
The integration of several types of data that originate from the same physical source (e.g.patient) but focus on different mechanisms (gene expression, DNA Methylation, histone modifications etc.) is an area of interest.

## Analysis of raw NGS data (.fastq)

- RNAseq (_HISAT2_)
- WES (_GATK_)
- ChIP-seq (_MACS2_)

## Downstream analysis

- differential analysis (_DEseq2_, _limma_)
- enrichment analysis (_KEGG_, _GO_)
- transciption factor binding site analysis (_PWA_)

## Data Integration
We developed a high-speed framework, called InterTADs, for integrating multi-omics data from the same physical source (e.g. patient) taking into account the chromatin configuration of the genome, i.e. the topologically associating domains (TADs). The main concept of the proposed methodology is to create a single matrix with all different events (e.g. DNA methylation, expression, mutation) combined with their genome coordinates and the respective quantitative metrics after application of the appropriate scaling. The events are divided into their related TADs according to the chromosomal location and each TAD is evaluated for statistically significant differences between the groups of interest (e.g. normal cells vs cancer cells). Finally, several visualization approaches are available, including the mapping of the events on the chromosomal location of the TAD as well as the distribution of the counts within a given TAD across the different study groups.

https://github.com/nikopech/InterTADs

