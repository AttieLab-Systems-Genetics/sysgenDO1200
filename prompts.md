# AI Prompts

## Prompts for README Files

- Create a [README.md](README.md) in `main_directory` that concisely summarizes contents at a high level.
- For `annotated_peak_summaries/README.md` parse filenames in this directory based on naming convention and add all found `phenotype_class` values to the unordered list in the `README.md` document. [Original attempt was too general and failed. User created starting document; AI filled out variables list, then refined by user.]
- Create a `mapping_data` [README.md](mapping_data/README.md) that concisely summarizes contents at a high level.
- Create a [README.md](README.md) in `scripts` that concisely summarizes contents at a high level. Include a link to `https://github.com/AttieLab-Systems-Genetics/mkeller3Projects2`.
- Create a `GitHub/README.md` that concisely summarizes contents at a high level.
- Update main_directory README with changes since it was last saved.
- For the main_directory README and the mapping_data README, add the last date modified in parentheses at the end of an item's description.

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
