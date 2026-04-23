# Mediation Analysis

This directory contains results from mediation analyses performed using the `bmediatR` package. Mediation analysis is a statistical technique used to identify potential causal intermediates (e.g., gene expression, protein levels) that lie on the biological pathway between a genetic locus (QTL) and a downstream phenotype.

## Directory Structure

The mediation results are organized into a multi-level hierarchy:

`mediations/[phenotype_class]/[trait_subset_and_model]/[mediator_set]/{in,out}put`

### 1. Phenotype Class
The category of the "target" trait being mediated:
- **`clinical_traits/`**: In vivo physiological measurements.
- **`liver_genes/`**: Liver gene expression (transcriptomics).
- **`liver_isoforms/`**: Liver isoform-level expression.
- **`liver_lipids/`**: Liver lipidomics.
- **`liver_metabolites_labeled/`**: Stable isotope labeled liver metabolites.
- **`plasma_metabolites/`**: Plasma metabolomics.
- **`liver_splice_juncs/`**: Alternative splicing events in the liver.

### 2. Trait Subset and Model
Defines the specific population of mice and the statistical model used for the target trait:
- e.g., `clinical_traits_all_mice_additive/`
- e.g., `liver_genes_qtlxdiet_in_HF_mice_additive/`

### 3. Mediator Set
The set of candidates being tested as potential mediators:
- **`mediator_set_liver_genes/`**: Testing all liver genes as potential causal intermediates.
- **`mediator_set_liver_isoforms/`**: Testing liver isoforms as potential intermediates.

### 4. Input and Output
- **`output/`**: Contains the primary result files:
  - **`mediation_[trait]_[chr]_[pos].csv`**: Ranks potential mediators by their probability of being a causal intermediate for a specific QTL peak.
  - **`mediation_log_file_[...].log`**: Execution logs for the mediation runs.
- **`input/`**: Contains configuration files and peak lists defining the mediation tasks.

## Summary and Reference Files

- **`all_mediation_summary_files/`**: Large-scale summary files that concatenate results across multiple peaks and phenotype classes for easier global analysis.
- **`bmediatR_output_definitions.md`**: Reference document explaining the column names and statistical metrics produced by the `bmediatR` pipeline.
