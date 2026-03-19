This folder contains the GitHub-specific files for the `main_directory`.

## Files

- [README_main_directory.md](README_main_directory.md): Overview of the `main_directory` folder.
- [README_annotated_peak_summaries.md](README_annotated_peak_summaries.md): Naming convention for peak summary files in `annotated_peak_summaries/` folder.
- [README_mapping_data.md](README_mapping_data.md): Overview of the `mapping_data` folder.
- [prompts.md](prompts.md): Prompts used for this and other documents.

## Symbolic Links

Each of these files has a
[symbolic link](https://www.computerhope.com/jargon/s/symblink.htm)
in the `main_directory` folder (or subfolder).
The symbolic links were created in Linix/MacOS using the following command:

```
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
