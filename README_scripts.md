# Analysis Scripts & Shiny Applications

This directory contains R scripts for data processing, QTL analysis, and interactive visualization using Shiny. These tools are designed for high-resolution mapping and functional annotation of genetic variants.

For the related code and collaborative development, visit the project repository:
[mkeller3Projects2](https://github.com/AttieLab-Systems-Genetics/mkeller3Projects2)

Dates of last documented change in parentheses (YYYY-MM-DD).

## QTL Mapping & Visualization

- **`QTL_Mapper_Functions.R`**: Core utility functions for the QTL mapping pipeline. (2026-03-16)
- **`Development of Manhattan  illustrating conservation of SNPs associated to our QTL.R`**: Script for generating Manhattan plots with conservation overlays. (2026-03-12)
- **`Shiny app to visualize a Manhattan plot of conservation... .R`**: Interactive Shiny applications (v1, v2, v3) for exploring SNP conservation and QTL results. (2026-03-12)
- **`launch shiny app to visualize SNP conservation.R`**: Helper script to launch the conservation visualization app. (2026-03-13)

## SNP Conservation & Annotation

- **`SNP_Indel_conservation_B6vSJL_variants.R`**: Analyzes conservation scores for specific B6 vs SJL variants. (2026-03-13)
- **`plot_mock_snp_conservation_35species_v7.R`**: Visualization script for multi-species SNP conservation. (2026-03-13)
- **`make_nfatc3_mock_cache_35species_v2.R`**: Pre-calculates data caches for the conservation visualization tools. (2026-03-13)

## Data Acquisition

- **`download_mm39_multiz35way_maf_to_W.R`**: Automated script for downloading multi-species alignment data (MAF format). (2026-03-13)

## Documentation

- **`README to launch QTL_Mapper_Functions R script.docx`**: Legacy documentation for the QTL mapping scripts. Content below is from this file. (2026-03-13)

1. Load the functions from the research drive

```r
source("W:/General/main_directory/scripts/QTL_Mapper_Functions.R") 
```

1. Launch the app

```r
launch_qtl_app()
```
