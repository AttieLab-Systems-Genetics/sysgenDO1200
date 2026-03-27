# Systems Genetics & QTL Mapping Pipeline

This directory contains the data, scripts, and results for a systems genetics pipeline focusing on Quantitative Trait Loci (QTL) mapping and mediation analysis. The project primarily utilizes mouse models (mm39) with orthologous mapping to human genomic data.
See [AI Prompts](prompts.md) for the prompts used for this and other documents. See additionally

- [annotated_peak_summaries/README.md](/GitHub/README_annotated_peak_summaries.md)
- [mapping_data/README.md](/GitHub/README_mapping_data.md)

## Directory Structure

### Data & Infrastructure

- **`raw_data/`**: Original input datasets.
- **`mapping_data/`**: Genotype and phenotype maps used for mapping.
- **`files_for_cross_object/`**: Files required to construct R/qtl2 cross objects.
- **`rankz_data/`**: Normalized and transformed phenotype data.
- **`ensembl_*.csv`**: Genomic reference files for mouse (GRCm39) and human (GRCh38).
- **`complete_meds_chr_18_61Mbp_locus.csv`**: Specific mediation results for the chromosome 18 locus.

### Analysis Steps

- **`scans/`**: Results of genome-wide scans (LOD scores).
- **`permutations/`**: Permutation test results for establishing significance thresholds.
- **`correlations/`**: Statistical correlations between traits and genotypes.
- **`mediations/`**: Outcomes of mediation analyses to identify causal candidates.
- **`snp_scans/`**: High-resolution association mapping results.
- **`output_directory/`**: General output results from various analysis steps.

### Annotation & Refinement

- **`top_snps_high_moderate_impact/`**: Variants filtered by high/moderate functional impact.
- **`top_snps_all_impact/`**: Variants filtered by all impact levels (low, moderate, high).
- **`variant_tables/`**: Detailed functional annotations for variants.
- **`annotated_peak_summaries/`**: Summarized results of significant QTL peaks.
- **`mm39_multiz35way_maf/`**: Multi-species alignment data for conservation scoring.

### Code & Documentation

- **`scripts/`**: R scripts for the analysis workflow and Interactive Shiny applications (e.g., QTL Fine-Mapper).
- **`Documentation/`**: Protocols, environment setup guides, and project overviews.
- **`R_package_source_files/`**: Local source code for project-specific R packages (`YandellIntermediate`).
- **`GitHub/`**: The git repository containing metadata and history for this project. This directory contains the source documentation files, which are symlinked to their respective locations in the project:
  - [`GitHub/README_main_directory.md`](GitHub/README_main_directory.md) -> `README.md`
  - [`GitHub/prompts.md`](GitHub/prompts.md) -> `prompts.md`
  - [`GitHub/README_annotated_peak_summaries.md`](GitHub/README_annotated_peak_summaries.md) -> `annotated_peak_summaries/README.md`
  - [`GitHub/README_mapping_data.md`](GitHub/README_mapping_data.md) -> `mapping_data/README.md`
  - [`GitHub/README.md`](GitHub/README.md): Overview of the GitHub repository and symlink setup.

## Getting Started

For an overview of the analysis workflow, refer to the documents in the `Documentation/` directory. To explore results interactively, see the Shiny apps provided in the `scripts/` folder.
