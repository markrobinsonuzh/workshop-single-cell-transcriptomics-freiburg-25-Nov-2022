# Workshop: Single Cell Transcriptomics

GitHub repository to collect all the materials for a workshop given by Mark D. Robinson at Uni. Freiburg 25.11.2022

# Some useful preliminaries

- Install [R 4.2.x](https://ftp.fau.de/cran/), [RStudio (now Posit)](https://posit.co/download/rstudio-desktop/)
- Install [Bioconductor 3.15 (or higher) packages](https://bioconductor.org/install/)
- Install [`quarto`](https://quarto.org/docs/get-started/hello/rstudio.html)
- Connect with [GitHub](https://github.com/) ?

# Install R/BioC packages

```
# more details at https://bioconductor.org/install/
install.packages("BiocManager")

BiocManager::install(version = "3.15")

pkgs <- c("DropletUtils", "SingleCellExperiment", "SingleR", "batchelor",
          "bluster", "dplyr", "edgeR", "ggplot2", "miloR", "muscat",
          "patchwork", "pheatmap", "scDblFinder", "scRNAseq", "scater",
          "scran", "scuttle","slingshot","tradeSeq")

BiocManager::install(pkgs)
BiocManager::valid()
```

# Download data from [here](https://www.dropbox.com/s/hwqx49qh6msa6ul/workshop-single-cell-transcriptomics-freiburg-25-Nov-2022-data.zip?dl=0)

# Some useful resources

- TODO: add links here

# Tentative schedule

| Time  | Topic | Material |
| --- |  --- | --- |
| 09.00-10.20  | preliminaries | session1_preliminaries |
| 10.20-10.40  | coffee break |  |
| 10.40-12.00  | QC, normalization, visualization | session2_qc-normalization-viz  |
| 12.00-13.00  | lunch break |  |
| 13.00-14.20  | differential abundance, differential state | session3_integation-da-ds |
| 14.20-14.40  | coffee break |  |
| 14.40-16.00  | trajectories, variations of DA/DS, wrap-up | session4_advanced |
| 16.00  | hard stop | |
| 16.13  | ICE75 @ Freiburg Hbf | |

# Notes

- The morning session was done with live coding; see [live_coding_25nov2022](live_coding_25nov2022)
- The afternoon session was done by going through my preparation scripts; see [demo_website](demo_website)
- Note to self: send `quarto` install instructions before hand; a few had issues installing it (e.g., needed new RStudio version)
- Some slides used were posted [here](scrnaseq-freiburg-workshop.pdf)
- Some notes collected in the YOPAD were cut/paste [here](cut-and-paste-from-yopad.txt)
