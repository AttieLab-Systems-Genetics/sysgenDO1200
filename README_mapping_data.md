# Mapping Data (DO1200 Cohort)

This directory contains the core genomic datasets and R/qtl2 objects required for QTL mapping, mediation analysis, and SNP association studies in the DO1200 cohort (GRCm39).

## Core R/qtl2 Objects

- **`cross_DO1200_grcm39.rds`**: The primary R/qtl2 `cross` object. It integrates phenotypes, genotypes, and covariates for the cohort. (2026-01-08)
- **`genoprobs_DO1200_grcm39.rds`**: Calculated genotype probabilities. (2024-11-04)
- **`alleleprobs_DO1200_grcm39.rds`**: Allele probabilities (8 founder states) derived from the genotype probabilities. (2024-11-04)
- **`snpprobs_DO1200_grcm39.rds`**: SNP probabilities mapped from founder variants for high-resolution association mapping. (2024-12-02)

## Kinship Matrices

Kinship matrices used to account for population structure during mapping:

- **`k_overall_DO1200_grcm39.rds`**: Global kinship matrix. (2025-01-20)
- **`k_chr_DO1200_grcm39.rds`**: Kinship matrices calculated per chromosome. (2025-01-20)
- **`k_loco_DO1200_grcm39.rds`**: Leave-one-chromosome-out (LOCO) kinship matrices. (2025-01-20)

## Performance & Optimization

- **`probs_fst/`**: Contains genotype, allele, and SNP probabilities stored in `fst` format. This allows for rapid, out-of-memory access to these large datasets (often many GBs in size) without exhausting system RAM. (2025-11-14)
- **`*_fstindex.rds`**: Index files used by the `fst` package to manage the out-of-memory data. (2026-01-05)

## Genotype Preparation & QC

- **`genotype_data_prep_and_QC/`**: Contains raw GigaMUGA data, founder consensus genotypes, and detailed quality control reports from the genotyping pipeline. (2026-01-26)
- **`liver_splice_junction_leafcutter_ids.csv`**: Reference mapping for splice junction identifiers used in transcriptomic mapping. (2025-04-01)

## Cleaned Data

- **`clean_genoprob_*.rds`**: Probability objects that have undergone additional filtering or cleaning steps post-calculation. (2026-01-05)
