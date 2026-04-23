# DO1200 Project Overview

This project is undertaken in the laboratory of
[Alan Attie](https://biochem.wisc.edu/people/attie/);
see
[Lab Website](https://attielab.biochem.wisc.edu/)
for overview of lab projects.

This specific project is known as DO1200, a name derived from the
[Diversity Outbred Mouse Population](https://pmc.ncbi.nlm.nih.gov/articles/PMC3524832/),
the source of the mice
This experiment aimed for 1200 mice, hence the name.

The key measurements concern genotypes (genetic characteristics at birth of each mouse) and phenotypes = traits (characteristics measured at various timepoints in the lives of each mouse).
An overarching goal is relating genotype to phenotype, in order to understand mechanisms of life processes such as metabolism and disease.

These measurements are combined through algorithms
developed over decades in the field of quantitative trait mapping.
These approximate relationships through statistical models, which are of necessity reductive and incomplete.
Analysis is typically done separately for each trait, with efforts to combine across traits based
on their inferred correlation through mapping to
nearby genetic positions, which are called quantitative trait loci or QTL.

Phenotypes are related based on how they measure
biological processes or physiological states,
including biochemical pathways that might be
altered or disrupted by genetic variation.
Genotypes are related due to proximity on the genome
as well as more complicated relationships due to
3D folding, evolutionary relationships among founders, and gene ontologies (for example).
The statistical methods oversimplify these
relationships, with subsequent heuristic approaches
hoping to capture relevant underlying biology.

The broader goal is to identify genes and regulatory elements that influence the
underlying biology.
A further complication is that the measured
traits are undoubtedly approximations of what
is biologically meaningful.

## Data Structures

Much of the data can be thought of as multiple tables
that are interconnected.
Some data characterize the individuals,
and other data provide measurements on those individuals.

### Genotypes and Phenotypes

The
[files_for_cross_object/README.md](main_directory/files_for_cross_object/README.md)
provides an overview of the files needed for mapping.
Genotypes relate subjects (mice) to marker positions along the genome.
Phenotypes (or traits)measure characteristics of each mouse,
possibly at various time points.
Covariates might be phenotypes, but are typically
determined by the design of the experiment.

The key structures are

- genotypes
  - genotypes (mouse or founder by marker)
  - genetic maps (marker by position)
  - physical maps (marker by position)
- phenotypes and covariates
  - phenotypes (mouse by trait)
  - covariates (mouse by covariate)
- annotations (genes, transcripts, markers, splice junctions)

### Peak Summaries

Summarized results of mapping (that is,
processed data) are stored in
[annotated_peak_summaries](main_directory/annotated_peak_summaries).
These summarize, over subjects (mice),
the QTL-based analyses of trait by position.
That is, for each trait, a score (LOD) is calculated for each genomic position
based on a mouse's imputed founder alleles.
The top (peak) per chromosome exceeding a threshold
is recorded.
The analysis can be done using several models,
which have additive effects of founder alleles
optionally plus interactions with sex and diet.

The peaks are actually regions rather than single
points.  
Several analyses of these regions are stored in

- peaks (trait by chromosome by model)
  - peak intervals (95% CI)
  - founder allele effects (founder by trait by chromosome)
- SNP associations (trait by chromosome by marker)

## SNP Scans

The markers are SNPs (single nucleotide polymorphisms), which divide the 8 founder
strains into two sets based on the strain
distribution pattern (SDP).
In additon to SNPs there are also indels (insertions and deletions) and other genetic markers.
SNP scans are in [snp_scans](main_directory/snp_scans).

While the summarized map results are based on the
additive effects of imputed founder alleles,
SNP scans consider the interactions
at the locus (additive and dominance effects).
That is, the SNP has 3 levels (A/A, A/B and B/B)
for the two SNP alleles.
These results complement but do not always
agree with the additive founder allele analyses.

SNP associations are computationally expensive
and are typically performed only at the peaks
once interesting loci are identified through
the additive founder allele analyses.

## Mediations

Mediation analysis tries to identify intermediate
processes that explain relationships between
genotype and phenotype.
Medations are in [mediations](main_directory/mediations).

Mediation analysis requires selection of mediators.
Current analysis uses liver genes and isoforms.
