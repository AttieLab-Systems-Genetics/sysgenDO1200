# Naming Convention for Peak Summary Files

This covers files in `annotated_peak_summaries/` and subdirectories.
The naming convention for files has [variables] that depend on the particular analysis.

- Peak Files in `.`
  - `DO1200_[phenotype_class]_[subjects]_mice_[model]_peaks.csv`
- Peak Files in `qtlxcovar_peaks/qtlxcov_peaks_in_splitby_additive_scans`
  - `DO1200_[phenotype_class]_qtlxdiet_peaks_in[subjects]_mice_[model].csv`
- LOD Profile Files in `lod_profile_rds_files`
  - `DO1200_[phenotype_class]_[subjects]_mice_[model]_lod_profiles.rds`
- LOD Profile Files in `qtlxcovar_peaks/lod_diff_profile_rds_files`
  - `DO1200_[phenotype_class]_[subjects]_mice_[qtlx]_lod_profiles.rds`

## Variables in File Names

- `phenotype_class`
  - `clinical_traits`
  - `liver_genes`
  - `liver_isoforms`
  - `liver_lipids`
  - `liver_metabolites_labeled`
  - `liver_splice_juncs`
  - `plasma_metabolites`
- `subjects`
  - `all`
  - `male`
  - `female`
  - `HC`
  - `HF`
- `model`
  - `additive`
  - `diet_interactive`
  - `sex_interactive`
  - `sexbydiet_interactive`
- `qtlx`
  - `qtlxdiet`
  - `qtlxsex`
  - `qtlxsexbydiet`
