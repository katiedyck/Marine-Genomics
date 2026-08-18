# MB5370 Module 3: Marine Genomics

This repository documents four computer workshops from the JCU MB5370 Marine Genomics module, working through the full pipeline of long-read (Oxford Nanopore) metagenome assembly — from raw reads to inferred metabolic pathways — using real and simulated data related to **Black Band Disease (BBD)**, a coral disease caused by a microbial mat community.

| Workshop | Topic | Summary |
------------------------------
| 1 | Introduction to Unix code in Rstudio | Getting familiar with the RStudio server environment, basic Unix commands (`pwd`, `ls`, `cd`, `mkdir`, `cat`, `head`, `grep`), and FASTA/FASTQ file formats. |
| 2 | Genome Assembly | Assembling a single bacterial isolate genome from long reads — read QC, running an assembler, and basic assembly statistics (N50, contig length/coverage). |
| 3 | Metagenome Assembly (mock community) | Assembling a _simulated_ 5-species mock bacterial community with `flye --meta`, exploring GC content/coverage to distinguish taxa, binning contigs with `metabat2`, and assessing bin quality with `checkm`. Introduces the two core challenges of metagenome assembly: variable species abundance and closely related strains/species. |
| 4 | Metagenome Assembly (real data) & Functional Analysis | Repeats the assembly → binning → quality-check pipeline on **real Nanopore sequencing data of Black Band Disease** (sampled from _Acropora hyacinthus_ at Orpheus Island), then adds taxonomic classification and functional/pathway analysis to ask _who_ is present in the BBD community and what they can do metabolically. |
--------------------------

- [Workshop 1](code/genomics_workshop1.Rmd) is an introduction to writing Unix code, the programming language used to write Terminal commands.
- [Workshop 2](code/genomics_workshop2.Rmd) covers genome assembly
- [Workshop 3](code/workshop3_MetagenomeAssembly.Rmd) covers metagenome assembly
- Workshop 4: [Black Band Disease (BBD)](code/workshop4_BBD.Rmd)

The [checkm](checkm), [flye](flye), [gtdbtk](gtdbtk), [metabat](metabat), [minpath](minpath) and [prokka](prokka) folders contain files from Workshop 4.

## Brief Description of Files and Folders

Figures and files generated during workshop 2 and workshop 3 are saved in folders `workshop2` and `workshop3`, respectively.

### [code](code) folder
- The [`styles.css`](code/styles.css) file contains formatting for my workshop 4 Markdown file that shows Terminal bash coding in a unique formatting, making it easier to distinguish from R coding.

Files and figures generated during workshop 4 can be found in the folders:
- `checkm` - 
- `flye` - 
- `gtdbtk` - 
- `metabat` - 
- `minpath` - 
- `prokka` - 
