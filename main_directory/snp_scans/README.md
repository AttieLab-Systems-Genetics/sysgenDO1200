# SNP Association Scans

This directory contains results from high-resolution SNP association mapping. Unlike the genome-wide QTL scans (which use founder allele probabilities), these scans perform association tests on individual SNPs at identified QTL peaks to refine candidate regions and identify potential causal variants.

## Directory Structure

The results are organized by phenotype class and mapping model:

`snp_scans/[phenotype_class]/[model]/{in,out}put`

### Phenotype Classes
- **`clinical_traits/`**: In vivo measurements (weight, GTT, lipids, etc.).
- **`liver_genes/`**: Gene expression data (transcriptomics).
- **`liver_isoforms/`**: Isoform-level expression data.
- **`liver_lipids/`**: Liver lipidomics data.
- **`liver_metabolites_labeled/`**: Stable isotope labeled metabolites in liver.
- **`plasma_metabolites/`**: Metabolomics data from plasma.

### Mapping Models
- **`all_mice_additive/`**: Standard additive model.
- **`all_mice_diet_interactive/`**: Model including interactions with diet.

## Folder Contents

### `output/` (Primary Results)

Contains the results of the SNP scans. The most relevant files for analysis are the `top_snps` summaries, which condense the full scan results for each peak:

- **`top_snps_[trait]_[chr]_[pos].csv`**: Summary of the strongest SNP associations for a given trait and peak location.
- **`top_snps_hi_mod_impact_[trait]_[chr]_[pos].csv`**: Summaries filtered for SNPs with "high" or "moderate" functional impact (e.g., missense variants, splice site changes).

These summary files include SNP identifiers, genomic coordinates (GRCm39), association scores, strain distribution patterns, and functional consequences.

### `input/`

Contains configuration and task list files used to drive the scanning pipeline:
- **`snp_scan_config_[N].yml`**: Pipeline parameters.
- **`run_these_qtl_[N].csv`**: The specific QTL peak regions targeted for high-resolution SNP mapping.

## Additional Summaries

- **`top_snps_counts_by_csq/`**: Statistical summaries of functional consequences (CSQ) for the top-scoring SNPs across large phenotype classes (e.g., all liver genes).
