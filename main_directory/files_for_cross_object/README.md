# Files for Cross Object

This directory contains input files required to build a `qtl2` cross object for the DO1200 project. These files include genotypes, genetic and physical maps, phenotypes, and annotations.

## Genotype Data

- **`geno_chr[N].csv`**: Genotype probabilities for each mouse across chromosomes 1-19, M, X, and Y.
- **`founder_geno_chr[N].csv`**: Founder genotype data for chromosomes 1-19, M, X, and Y.

## Map Data

- **`gmap_chr[N].csv`**: Genetic maps for chromosomes 1-19, M, X, and Y.
- **`pmap_chr[N].csv`**: Physical maps for chromosomes 1-19, M, X, and Y.

## Phenotype Data

These files contain various measurements across the DO1200 mice:

- **`pheno_in_vivo_clinical_traits_v3.csv`**: Clinical traits measured in vivo.
- **`pheno_liver_13C_metabolites_*.csv`**: 13C fractional enrichments for liver metabolites (POS and NEG columns).
- **`pheno_liver_2H_metabolites_fractional_enrichments_DO_diet.csv`**: 2H fractional enrichments for liver metabolites.
- **`pheno_liver_genes_DO_diet_nonzero150_vsd_v3.csv`**: Liver gene expression data.
- **`pheno_liver_isoforms_DO_diet_nonzero150_vsd_v3.csv`**: Liver isoform expression data.
- **`pheno_liver_lipids_combat_corrected.csv`**: Batch-corrected liver lipidomics.
- **`pheno_liver_psi_DO_diet_nonzero150_qqnorm_v2.csv`**: Liver alternative splicing (PSI) data.
- **`pheno_plasma_13C_metabolite_GTT_metatraits_DO_diet_batch_corrected.csv`**: Plasma 13C GTT metatraits.
- **`pheno_plasma_2H_metabolite_GTT_metatraits_DO_diet_batch_corrected.csv`**: Plasma 2H GTT metatraits.

## Covariates

- **`covar.csv`**: General covariates for the analysis.
- **`phenocovar.csv`**: Phenotype-specific covariates.

## Annotations

- **`gene_annotations.csv`**: Information about genes.
- **`transcript_annotations.csv`**: Information about transcripts.
- **`marker_annotations_DO_diet_grcm39.csv`**: Marker positions and details (GRCm39).
- **`liver_splice_junction_annotations.csv`**: Details on splice junctions in liver data.

## Configuration and Metadata

- **`control_file.json`**: JSON file containing metadata and paths for loading the cross object.
- **`chromosomal_sep_grcm39.csv`**: Chromosomal separation info.
- **`version_log.rds`**: Log of data versions and changes.
- **`k_loco_DO1200_grcm39.rds`**: Kinship matrix (Leave-One-Chromosome-Out method).
