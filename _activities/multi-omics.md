---
title: 'Multi-omics'
image: '/activities/default.png'
---

The Next Generation Sequencing (NGS) produce big biological data. The process of analyzing omics data usually leads to a high dimensional matrix, with the different cases listed as columns and the locations on the genome in which the examined event happened (e.g. mutation, gene expression etc.) as rows.

The particular omics computational approaches currently in progress fall in the biomedical domain include:

1. High throughput immunogenetic analysis in health and disease
2. Integrated omics analysis of hematologic malignancies: DNA methylome and Transcriptome Profiling in patients with hematologic malignancies treated with chemotherapy versus novel agents; Whole exome sequencing of pre-malignant conditions
3. Targeted NGS analysis for improved risk stratification in cancer: novel recurrent gene mutations in hematologic malignancies


## Analysis of raw NGS data (.fastq)

- Immuno-sequencing (_IMGT_)
- RNAseq (_HISAT2_)
- WES (_GATK_)
- ChIP-seq (_MACS2_)

## Downstream analysis

- Immunogetics analysis (_TRIP - T cell receptor/immunoglobulin profiler_)
- differential analysis (_DEseq2_, _limma_)
- enrichment analysis (_KEGG_, _GO_)
- transciption factor binding site analysis (_PWA_)

## Data Integration
We developed a high-speed framework, called InterTADs, for integrating multi-omics data from the same physical source (e.g. patient) taking into account the chromatin configuration of the genome, i.e. the topologically associating domains (TADs).
[Check it out on our github](https://github.com/nikopech/InterTADs)

