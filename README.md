# Differential-RNA-expression-analysis
BI practicum 6

This lab report demonstrates changes that happen in yeast cells before or during fermentation.

This repository contains a jupyter notebook where the workflow is described and a .pdf file with the lab report. 

We will explore how RNA expression levels change as yeast undergo fermentation to make bread rise. There are two replicates of RNA-seq data from yeast before and during fermentation, and our goal is to find out if the yeast express different genes during fermentation than they do under normal growth.

## Data

This lab work uses the following data:
- yeast reads: \
  [SRR941816](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR941/SRR941816/SRR941816.fastq.gz): fermentation 0 minutes replicate 1 (413 Mb) \
  [SRR941817](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR941/SRR941817/SRR941817.fastq.gz): fermentation 0 minutes replicate 2 (455 Mb) \
  [SRR941818](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR941/SRR941818/SRR941818.fastq.gz): fermentation 30 minutes replicate 1 (79.3 Mb) \
  [SRR941819](http://ftp.sra.ebi.ac.uk/vol1/fastq/SRR941/SRR941819/SRR941819.fastq.gz): fermentation 30 minutes replicate 2 (282 Mb) 
- [reference genome file](http://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/146/045/GCF_000146045.2_R64/GCF_000146045.2_R64_genomic.fna.gz)
- [annotation file](http://ftp.ncbi.nlm.nih.gov/genomes/all/GCF/000/146/045/GCF_000146045.2_R64/GCF_000146045.2_R64_genomic.gff.gz)

## Key results

Differential expression was obtained for RNA-seq data. Following heatmap with the results was plotted

![heatmap](output.pdf)

## Usage

To reproduce the enviroment use:
```bash
conda env create -f environment.yml
conda activate prac_hw6
```
