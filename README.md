# Systems Genetics & QTL Mapping Pipeline

This directory contains the data, scripts, and results for a systems genetics pipeline focusing on Quantitative Trait Loci (QTL) mapping and mediation analysis. The project primarily utilizes mouse models (mm39) with orthologous mapping to human genomic data.
See [AI Prompts](prompts.md) for the prompts used for this and other documents. See additionally

- [annotated_peak_summaries/README.md](annotated_peak_summaries/README.md)
- [mapping_data/README.md](mapping_data/README.md)

## Directory Structure

### Data & Infrastructure

- **`raw_data/`**: Original input datasets.
- **`mapping_data/`**: Genotype and phenotype maps used for mapping.
- **`files_for_cross_object/`**: Files required to construct R/qtl2 cross objects.
- **`rankz_data/`**: Normalized and transformed phenotype data.
- **`ensembl_*.csv`**: Genomic reference files for mouse (GRCm39) and human (GRCh38).

### Analysis Steps

- **`scans/`**: Results of genome-wide scans (LOD scores).
- **`permutations/`**: Permutation test results for establishing significance thresholds.
- **`correlations/`**: Statistical correlations between traits and genotypes.
- **`mediations/`**: Outcomes of mediation analyses to identify causal candidates.
- **`snp_scans/`**: High-resolution association mapping results.

### Annotation & Refinement

- **`top_snps_high_moderate_impact/`**: Variants filtered by functional impact.
- **`variant_tables/`**: Detailed functional annotations for variants.
- **`annotated_peak_summaries/`**: Summarized results of significant QTL peaks.
- **`mm39_multiz35way_maf/`**: Multi-species alignment data for conservation scoring.

### Code & Documentation

- **`scripts/`**: R scripts for the analysis workflow and Interactive Shiny applications (e.g., QTL Fine-Mapper).
- **`Documentation/`**: Protocols, environment setup guides, and project overviews.
- **`R_package_source_files/`**: Local source code for project-specific R packages (`YandellIntermediate`).

## Getting Started

For an overview of the analysis workflow, refer to the documents in the `Documentation/` directory. To explore results interactively, see the Shiny apps provided in the `scripts/` folder.
