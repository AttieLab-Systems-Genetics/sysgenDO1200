# AI Prompts

## Prompts for README Files

- Create a [README.md](README.md) in `main_directory` that concisely summarizes contents at a high level.
- For `annotated_peak_summaries/README.md` parse filenames in this directory based on naming convention and add all found `phenotype_class` values to the unordered list in the `README.md` document. [Original attempt was too general and failed. User created starting document; AI filled out variables list, then refined by user.]
- Create a `mapping_data` [README.md](mapping_data/README.md) that concisely summarizes contents at a high level.
- Create a [README.md](scripts/README.md) in `scripts` that concisely summarizes contents at a high level. Include a link to `https://github.com/AttieLab-Systems-Genetics/mkeller3Projects2`.
- Create a `GitHub/README.md` that concisely summarizes contents at a high level.
- Update main_directory README with changes since it was last saved.
- For the main_directory README and the mapping_data README, add the last date modified in parentheses at the end of an item's description.
- In GitHub, create a README.md for `files_for_cross_object/` that concisely summarizes contents at a high level. This  should condense information that has multiple similar files, such as `geno_chrN.csv` for N = 1..19,M,X,Y`.
Match the folder structure of`main_directory/files_for_cross_object/` in `GitHub/main_directory/files_for_cross_object/` and create symbolic link in `files_for_cross_object/` to point to the README.md file in GitHub.
- In GitHub/main_directory/snp_scans`, create a [README.md](README.md) that concisely summarizes contents at a high level. This should condense information that has multiple similar files.
Note that this folder has hierarchy`[phenotype_class]/[model]/{in,out}put`;
the`top_snps` files in `output` are the most relevant for analysis.
Match the folder structure of `main_directory/snp_scans/` in `GitHub/main_directory/snp_scans/` and create symbolic link in `snp_scans/` to point to the README.md file in GitHub.
- Similar README for `main_directory/mediations/`.

## Symbolic Links from GitHub Folder

I have created symbolic links from the GitHub folder to main_directory and subfolders as follows:

```bash
ln -s GitHub/main_directory/README.md README.md
ln -s GitHub/prompts.md prompts.md

cd annotated_peak_summaries
ln -s ../GitHub/main_directory/annotated_peak_summaries/README.md README.md

cd ../mapping_data
ln -s ../GitHub/main_directory/mapping_data/README.md README.md

cd ../scripts
ln -s ../GitHub/main_directory/scripts/README.md README.md
```

I have now created a `main_directory` subfolder of `GitHub`, with subfolders for each of the major subfolders of `main_directory`.
Rearrange, rename and re-link main `README_*.md` files in `main_directory` and subfolders to match this nested directory structure.

## Data Structures

Develop a new markdown file in GitHub that
