# Module 07 — GVA & GWAS with Population Structure

## Overview

This repository contains the completed work for Module 07, including:

1. **E. coli variant analysis and circos plot**
2. **GWAS analysis with population structure**

---

## 1. E. coli Variant Circos Plot

The E. coli variant analysis uses sequencing reads mapped to the *E. coli* reference genome **NC_012967.1**.

The workflow includes:

* Quality trimming of paired-end sequencing reads
* Mapping reads to the reference genome
* Processing mapped reads into a sorted BAM file
* Variant calling using `bcftools`
* Generation of a VCF containing identified variants
* Visualization of variant positions using a circos plot

The final circos plot illustrates the positions of coding and non-coding variants across the E. coli genome.

### Input Data

* `NC_012967.1.fasta`
* `SRR030257_1.fastq`
* `SRR030257_2.fastq`

### Variant Output

The variant-calling workflow produces:

```text
trimmed_reads.vcf
```

---

## 2. GWAS Tutorial with Population Structure

The GWAS analysis uses genotype and phenotype data to identify associations between genetic variants and the phenotype while accounting for population structure.

The analysis uses:

* `genotypes.vcf`
* `phenotypes.tsv`

Population structure is accounted for using principal components (PCs) as covariates in the association analysis.

The completed notebook is:

```text
GWAS_Tutorial.ipynb
```

The final analysis includes:

* Population structure analysis
* Principal component analysis
* Population-structure-adjusted GWAS
* QQ plot
* Manhattan plot

The final QQ and Manhattan plots show the GWAS results after accounting for population structure.

---

## Repository Contents

```text
Bioinformatics_Module07_GWAS/
│
├── README.md
└── GWAS_Tutorial.ipynb
```

---

## Module 07 Submission

The completed `GWAS_Tutorial.ipynb` is provided in this repository as the submission artifact for the GWAS portion of Module 07.

A fixed GitHub release contains the submitted version of the completed notebook.
