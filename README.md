# MB5370 Module 3: Marine Genomics

This repository documents four computer workshops from the JCU MB5370 Marine Genomics module, working through the full pipeline of long-read (Oxford Nanopore) metagenome assembly — from raw reads to inferred metabolic pathways — using real and simulated data related to **Black Band Disease (BBD)**, a coral disease caused by a microbial mat community.

| Workshop | Topic | Summary |
| :---- | :---- | :---- |
| 1 | Introduction to Unix code in Rstudio | Getting familiar with the RStudio server environment, basic Unix commands (`pwd`, `ls`, `cd`, `mkdir`, `cat`, `head`, `grep`), and FASTA/FASTQ file formats. |
| 2 | Genome Assembly | Assembling a single bacterial isolate genome from long reads — read QC, running an assembler, and basic assembly statistics (N50, contig length/coverage). |
| 3 | Metagenome Assembly (mock community) | Assembling a _simulated_ 5-species mock bacterial community with `flye --meta`, exploring GC content/coverage to distinguish taxa, binning contigs with `metabat2`, and assessing bin quality with `checkm`. Introduces the two core challenges of metagenome assembly: variable species abundance and closely related strains/species. |
| 4 | Metagenome Assembly (real data) & Functional Analysis | Repeats the assembly → binning → quality-check pipeline on **real Nanopore sequencing data of Black Band Disease** (sampled from _Acropora hyacinthus_ at Orpheus Island), then adds taxonomic classification and functional/pathway analysis to ask _who_ is present in the BBD community and what they can do metabolically. |
--------------------------

Workshops 1–3 focus on core skills (Unix, R, assembly, binning, QC) using either no data or a simplified mock community. Workshop 4 is the assessable piece — it applies the full pipeline to a real disease metagenome and pushes into functional annotation and pathway inference.

## Brief Description of Files and Folders

Figures and files generated during workshop 2 and workshop 3 are saved in folders `workshop2` and `workshop3`, respectively.

### [code](code) folder
- Contains the R Markdown files for each workshop, along with their html outputs.
- The [`styles.css`](code/styles.css) file contains formatting for my workshop 4 Markdown file that shows Terminal bash coding in a unique formatting, making it easier to distinguish from R coding.

Workshop 4 works through the BBD metagenome in a sequence of steps, each producing its own folder. The pipeline flows in this order:
`flye` → `metabat` → `checkm` → `gtdbtk` / `prokka` → `minpath`

`flye/`
