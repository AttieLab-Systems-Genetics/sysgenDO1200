This repo contains documentation files for the [ResearchDrive](https://it.wisc.edu/services/researchdrive/)
folder `mkeller3/General/main_directory`.
The repo is a mirror of the subfolder `GitHub`.
This repo is private, as is the ResearchDrive area.

## Files

- [README_main_directory.md](README_main_directory.md): Overview of the `main_directory` folder.
- [README_annotated_peak_summaries.md](README_annotated_peak_summaries.md): Naming convention for peak summary files in `annotated_peak_summaries/` subfolder.
- [README_mapping_data.md](README_mapping_data.md): Overview of the `mapping_data` subfolder.
- [prompts.md](prompts.md): Prompts used for this and other documents.

## Symbolic Links

Each of these files has a
[symbolic link](https://www.computerhope.com/jargon/s/symblink.htm)
in the `main_directory` folder (or subfolder).
The symbolic links enable us to have the main copy of the material in the GitHub folder, while still having the documentation easily accessible (as mirrors) in `main_directory`
and subfolders.
The symbolic links were created in Linix/MacOS using the following command:

```bash
cd main_directory
ln -s GitHub/README_main_directory.md README.md
ln -s GitHub/prompts.md prompts.md

cd annotated_peak_summaries
ln -s ../GitHub/README_annotated_peak_summaries.md README.md

cd ../mapping_data
ln -s ../GitHub/README_mapping_data.md README.md
```

- [README_main_directory.md](../README.md)
- [README_annotated_peak_summaries.md](../annotated_peak_summaries/README.md)
- [README_mapping_data.md](../mapping_data/README.md)
