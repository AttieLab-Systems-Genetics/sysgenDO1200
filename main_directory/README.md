# Systems Genetics & QTL Mapping Pipeline

This directory contains the data, scripts, and results for a systems genetics pipeline focusing on Quantitative Trait Loci (QTL) mapping and mediation analysis. The project primarily utilizes mouse models (mm39) with orthologous mapping to human genomic data.
See [AI Prompts](prompts.md) for the prompts used for this and other documents.
Dates of last documented change in parentheses (YYYY-MM-DD).
See additionally

- [annotated_peak_summaries/README.md](annotated_peak_summaries/README.md)
- [mapping_data/README.md](mapping_data/README.md)
- [scripts/README.md](scripts/README.md)

## Directory Structure

### Data & Infrastructure

- **`raw_data/`**: Original input datasets. (2026-03-19)
- **`mapping_data/`**: Genotype and phenotype maps used for mapping. (2026-03-18)
- **`files_for_cross_object/`**: Files required to construct R/qtl2 cross objects. (2026-02-26)
- **`rankz_data/`**: Normalized and transformed phenotype data. (2026-01-16)
- **`ensembl_*.csv`**: Genomic reference files for mouse (GRCm39) and human (GRCh38). (2026-02-04)
- **`complete_meds_chr_18_61Mbp_locus.csv`**: Specific mediation results for the chromosome 18 locus. (2025-06-11)

### Analysis Steps

- **`scans/`**: Results of genome-wide scans (LOD scores). (2026-03-25)
- **`permutations/`**: Permutation test results for establishing significance thresholds. (2026-02-26)
- **`correlations/`**: Statistical correlations between traits and genotypes. (2026-02-05)
- **`mediations/`**: Outcomes of mediation analyses to identify causal candidates. (2026-01-08)
- **`snp_scans/`**: High-resolution association mapping results. (2026-02-02)
- **`output_directory/`**: General output results from various analysis steps. (2026-01-19)

### Annotation & Refinement

- **`top_snps_high_moderate_impact/`**: Variants filtered by high/moderate functional impact. (2026-02-03)
- **`top_snps_all_impact/`**: Variants filtered by all impact levels (low, moderate, high). (2026-03-26)
- **`variant_tables/`**: Detailed functional annotations for variants. (2026-03-26)
- **`annotated_peak_summaries/`**: Summarized results of significant QTL peaks. (2026-03-26)
- **`mm39_multiz35way_maf/`**: Multi-species alignment data for conservation scoring. (2026-03-13)

### Code & Documentation

- **`scripts/`**: R scripts for the analysis workflow and Interactive Shiny applications (e.g., QTL Fine-Mapper). (2026-03-13)
- **`Documentation/`**: Protocols, environment setup guides, and project overviews. (2025-12-04)
- **`R_package_source_files/`**: Local source code for project-specific R packages (`YandellIntermediate`). (2024-11-07)
- **`GitHub/`**: The git repository containing metadata and history for this project. This directory contains the source documentation files, which are symlinked to their respective locations in the project: (2026-03-22)
  - `GitHub/README_main_directory.md` -> `README.md`
  - `GitHub/prompts.md` -> `prompts.md`
  - `GitHub/README_annotated_peak_summaries.md` -> `annotated_peak_summaries/README.md`
  - `GitHub/README_mapping_data.md` -> `mapping_data/README.md`
  - `GitHub/README_scripts.md` -> `scripts/README.md`
  - `GitHub/README.md`: Overview of the GitHub repository and symlink setup.

## Getting Started

For an overview of the analysis workflow, refer to the documents in the `Documentation/` directory. To explore results interactively, see the Shiny apps provided in the `scripts/` folder.
