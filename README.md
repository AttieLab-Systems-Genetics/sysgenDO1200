# GitHub Documentation Repository

This repo contains documentation files for the [ResearchDrive](https://it.wisc.edu/services/researchdrive/)
folder `mkeller3/General/main_directory`.
The repo is a mirror of the subfolder `GitHub`.
This repo is public, but the ResearchDrive (RD) area is private.
The file
[project.md](project.md)
describes the project in more detail.

## Files

- [project.md](project.md): Outline of project.
- [main_directory/README.md](main_directory/README.md): Overview of the `main_directory` folder.
- [main_directory/annotated_peak_summaries/README.md](main_directory/annotated_peak_summaries/README.md): Naming convention for peak summary files in `annotated_peak_summaries` subfolder.
- [main_directory/mapping_data/README.md](main_directory/mapping_data/README.md): Overview of the `mapping_data` subfolder.
- [main_directory/scripts/README.md](main_directory/scripts/README.md): Overview of the `scripts` subfolder.
- [main_directory/files_for_cross_object/README.md](main_directory/files_for_cross_object/README.md): Overview of the `files_for_cross_object` subfolder.
- [main_directory/snp_scans/README.md](main_directory/snp_scans/README.md): Overview of the `snp_scans` subfolder.
- [main_directory/mediations/README.md](main_directory/mediations/README.md): Overview of the `mediations` subfolder.
- [prompts.md](prompts.md): Prompts used for this and other documents.

## Symbolic Links

Each of these files has a
[symbolic link](https://www.computerhope.com/jargon/s/symblink.htm)
in the `main_directory` folder (or subfolder).
The symbolic links enable us to have the main copy of the material in the GitHub folder, while still having the documentation easily accessible (as mirrors) in `main_directory`
and subfolders.
The symbolic links were created in Linix/MacOS using the following command:

```bash
ln -s GitHub/main_directory/README.md README.md
ln -s GitHub/prompts.md prompts.md

cd annotated_peak_summaries
ln -s ../GitHub/main_directory/annotated_peak_summaries/README.md README.md

cd ../mapping_data
ln -s ../GitHub/main_directory/mapping_data/README.md README.md

cd ../scripts
ln -s ../GitHub/main_directory/scripts/README.md README.md

cd ../files_for_cross_object
ln -s ../GitHub/main_directory/files_for_cross_object/README.md README.md

cd ../snp_scans
ln -s ../GitHub/main_directory/snp_scans/README.md README.md

cd ../mediations
ln -s ../GitHub/main_directory/mediations/README.md README.md
```

- [main_directory/README.md](../README.md)
- [main_directory/annotated_peak_summaries/README.md](../annotated_peak_summaries/README.md)
- [main_directory/mapping_data/README.md](../mapping_data/README.md)
- [main_directory/scripts/README.md](../scripts/README.md)
- [main_directory/files_for_cross_object/README.md](../files_for_cross_object/README.md)
- [main_directory/snp_scans/README.md](../snp_scans/README.md)
- [main_directory/mediations/README.md](../mediations/README.md)

---

I connected the `GitHub` folder on RD with this GitHub repository (or "repo")
using help from
[Get started with GitHub](https://happygitwithr.com/usage-intro#usage-intro).
Specifically, I created the RD folder and used instructions about
[Existing project, GitHub last](https://happygitwithr.com/existing-github-last#existing-github-last)
to set up the connection.
