# An updated Bioconductor workflow for correlation profiling subcellular proteomics

This Github repository contains the text, code and data for the workflow written by Hutchings et al., entitled "An updated Bioconductor workflow for correlation profiling subcellular proteomics", submitted to F1000Research 12th May 2025.

Data:

* The raw mass spectrometry data for the LOPIT-DC use-case in the main workflow can be found on the PRIDE database under the identifier [PXD055123](https://proteomecentral.proteomexchange.org/cgi/GetDataset?ID=PXD055123)
* The necessary files to run the main workflow are the PSM and protein-level output files (a549_uv_lopit_PSMs.txt and a549_uv_lopit_Proteins.txt) from an identification search carried out with Proteome Discoverer v3.1, along with a list of subcellular markers (mrk.csv). These can be found at Zenodo under the [doi: 10.5281/zenodo.15100485](http://doi.org/10.5281/zenodo.15100485).
* Since some of the later machine learning steps require additional computational time and power, we also provide some intermediate objects containing the outputs of these code chunks so that users can directly load and look at these without running the code locally. These objects are the final QFeatures object (qf.rda) and output of running the TAGM-MCMC (tagm_mcmc_params.rda) and BANDLE algorithms (bandleres.rda). These can be found at Zenodo under the [doi: 10.5281/zenodo.15100485](http://doi.org/10.5281/zenodo.15100485).
* For the appendix, the raw mass spectrometry data for the DIA correlation profiling use-case can be found on the PRIDE database under the identifier PXD063082
* The necessary files to run the example DIA correlation profiling workflow presented in the appendix are the output report file (diann_report.tsv) from a library-free DIA-NN identification search and the contaminant fasta file included in this search (220813_Universal_Protein_Contaminants_HaoGroup_modified.fasta). These can be found at Zenodo under the [doi: 10.5281/zenodo.15100485](http://doi.org/10.5281/zenodo.15100485).

Manuscript:

* The workflow is available in R Markdown and PDF in the [main repo](https://github.com/CambridgeCentreForProteomics/f1000_subcellular_proteomics)
* The accompanying appendix is also available as a PDF in the [main repo](https://github.com/CambridgeCentreForProteomics/f1000_subcellular_proteomics)
  

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
