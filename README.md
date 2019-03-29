# KFERQ_analysis

## This repository contains the scripts used for the analysis of KFERQ-like CMA targeting in the human proteome.

The scripts are arranged according to the figures in Kirchner et. al. 2019. Since later figures build on the data of previous ones scripts should be run in order to ensure all necessary intermediate files are generated.  
  
The raw proteome data is provided for human. For a new proteome, the first code chunk in Figure 1 builds the necessary data from a R data object (.Rds) containing the necessary information (protein ID, length, sequence) and saves it as an R data object.  
The proteome and motif tables are then used to build all necessary tables for the following analyses. Some particular steps, like the enrichment analysis require require additional data, in this case the GO-term annotation column from UniProtKB.  

## raw data for figures
The raw data do rebuild the figures is located in the folder "raw_data_figures" as .csv tables

## further raw data
The relevant raw data to retrace the analysis script can be found in the archive "raw_data.tar.gz":  
  
**human_proteome** UniProtKB human proteome (UP000005640), downloaded 1/16/2018  
**human_CMA_motifs** CMA motifs identified in the human proteome  
**motif_modification_reference** (contains information about all possible KFERQ-like motifs)  
**known_substrates_motivs** CMA motifs identified in known CMA substrates  
**known_substrates_output_jnet** JPred4 prediction results for the known CMA substrates  
**confirmed_motifs** pdb structres and structure predictions for known CMA substrates  
**one_canon_output_jnet** JPred4 prediction results for proteins with one single canonical motif  
**L2A100_3K.json** (result of the BLAST search for LAMP-2A isoforms)  
**species_tree_for_conservation** (taxonomic IDs of the CMA-able and unable species)  
**EggNOG_identifiers.txt** (used to translate from UniProt to EggNOG IDs)  
**newGO_custom_names.csv** (list of GO terms used for the enrichment analysis)  
**map2slim_output_tsv.txt** (mapping of child GO terms to the specified parent terms)  
**ratios_list.json** (mapping of the fractional motif content into bins for the triangle plots)  
**conf_motifs** (folder containing structural information for the experimentally confirmed CMA substrates)  

