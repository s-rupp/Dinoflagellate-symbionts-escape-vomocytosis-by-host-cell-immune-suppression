# Dinoflagellate-symbionts-escape-vomocytosis-by-host-cell-immune-suppression

For running scripts the following packages need to be installed in R!
Scripts were run in R version 4.0.3

From Bioconductor:

if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(c("Biobase", "KEGGREST", "DESeq2", "ComplexHeatmap", "qvalue", "HilbertCurve", "IRanges", "pathview"))


From CRAN:
install.packages("clustr", "readr", "dplyr", "knitr", "circlize", "grDevices", "colorRamps", "mgcv", "ggplot2", "ggsignif", "emmeans", "tidyr", "plyr")



For Figures 1d, 1e, 2b, 2d, 2e, 2f, 3a, 3b, 3c, 3e, 5a, 5b, 5c, 5d, (S1), S2 :

Raw data, R scripts and resulting tables and images can be found in the respective folders. 




For Figure 4 a:

Knime workflow was run in version Knime version 4.3.1

Needed extension:
	KNIME Interactive R Statistics Integration	 (Tested version: 4.3.1.v202101261634)

For R integration to work, rserve >v1.8.6 needs to be installed in R (from CRAN)


Data needed (and written) can be found in Folder "RNA_seq", which needs to be copied to the same folder the Knime workflow is imported to (usually the knime LOCAL folder).

XP2XM.csv file was extracted from NCBI anotation data in 2018, a current (updated) version can be found at (be aware that anotations have changed and do not fit to our mapping of reads):

https://ftp.ncbi.nlm.nih.gov/genomes/refseq/invertebrate/Exaiptasia_diaphana/annotation_releases/101/GCF_001417965.1_Aiptasia_genome_1.1/

epa2ko.csv and XP2epa.csv were created in R with KEGGREST in 2018.
Current versions (updated to fit to new NCBI anotations) can be created as with the Rscript in Folder "Kegg_accession_numbers". 


For Figure 4b:

Figure 4b is based on Kegg pathways as created with pathview in R. 
Source data was created in the Figure4a knime workflow --> to ../RNA_seq/pathview.csv
This file was copied to the Figure4b_data folder for R.



Extended Data Table 2 was created in Figure4a Knime workflow.







