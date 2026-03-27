# Analysis Scripts & Shiny Applications

This directory contains R scripts for data processing, QTL analysis, and interactive visualization using Shiny. These tools are designed for high-resolution mapping and functional annotation of genetic variants.

Dates of last documented change in parentheses (YYYY-MM-DD).

## Contents

- [QTL Mapping & Visualization](#qtl-mapping--visualization)
- [SNP Conservation & Annotation](#snp-conservation--annotation)
- [Data Acquisition](#data-acquisition)
- [Documentation](#documentation)
- [Additional Code on ResearchDrive and GitHub](#additional-code-on-researchdrive-and-github)

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

## Additional Code on ResearchDrive and GitHub

The overview above is for the [ResearchDrive (RD)](https://it.wisc.edu/services/researchdrive/)
folder `mkeller3/General/main_directory/scripts`.

Additional code on RD can be found in

- `mkeller3/General/Projects2/` (Mark Keller)
  - `mkeller3/General/Projects2/R scripts` (see repo
[AttieLab-Systems-Genetics/mkeller3Projects2](https://github.com/AttieLab-Systems-Genetics/mkeller3Projects2))
  - `mkeller3/General/Projects2/Antigravity` (mix of code and processed data)
- `mkeller3/General/emfinger_ML_projects` (Chris Emfinger)
- `mkeller3/General/QTL_mapping_KM` (Kelly Mitok)
  - `mkeller3/General/QTL_mapping_KM/scripts` (Kelly Mitok)
- `mkeller3/General/VEP/scripts` (??)
- ?? (Charles Opara)
- Box folder (Alan Attie)

Additional code on GitHub can be found in
[AttieLab-Systems-Genetics](https://github.com/AttieLab-Systems-Genetics).
See the list of repositories at
[AttieLab-Systems-Genetics](https://github.com/orgs/AttieLab-Systems-Genetics/repositories).
