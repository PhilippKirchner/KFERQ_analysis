#KFERQ_analysis

##This repository contains the scripts used for the analysis of KFERQ-like CMA targeting in the human proteome.  
  
The scripts are arranged according to the figures in Kirchner et. al. XXXX. Since later figures build on the data of previous ones scripts should be run in order to ensure all necessary intermediate files are generated.  
  
The raw proteome data is not provided. The first code chunk in Figure 1 builds the necessary data from a R data object (.Rds) containing the necessary information (protein ID, length, sequence) and saves it as an R data object. This information is used to build all necessary tables later on. For later analyses the GO-term annotation column from the UniProtKB is required.  
  
Data included in this repository are:  
*motif_modification_reference* (contains information about all possible KFERQ-like motifs).  
*L2A100_3K.json* (result of the BLAST search for LAMP-2A isoforms)
*species_tree_for_conservation* (taxonimic IDs of the CMA-able and unable species).  
*EggNOG_identifiers.txt* (used to translate from UniProt to EggNOG IDs).  
*newGO_custom_names.csv* (list of GO terms used for the enrichment analysis).  
*map2slim_output_tsv.txt* (mapping of child GO terms to the specified parent terms).  
*ratios_list.json* (mapping of the fractional motif content into bins for the triangle plots).  
*conf_motifs* (folder containing structural information for the experimentally confirmed CMA substrates)  

