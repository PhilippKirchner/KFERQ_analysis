# KFERQ_analysis

## This repository contains the scripts used for the analysis of KFERQ-like CMA targeting in the human proteome.

The scripts are arranged according to the figures in Kirchner et. al. 2019. Since later figures build on the data of previous ones scripts should be run in order to ensure all necessary intermediate files are generated.  
  
The raw proteome data is provided for human. For a new proteome, the first code chunk in Figure 1 builds the necessary data from a R data object (.Rds) containing the necessary information (protein ID, length, sequence) and saves it as an R data object.  
The proteome and motif tables are then used to build all necessary tables for the following analyses. Some particular steps, like the enrichment analysis require require additional data, in this case the GO-term annotation column from UniProtKB.  

## raw data for figures
The raw data do rebuild the figures is located in the folder "raw_data_figures" as .csv tables

## further raw data
The relevant raw data to retrace the analysis script can be found in the archive "raw_data.zip":  
  
**human_proteome** UniProtKB human proteome (UP000005640), downloaded 1/16/2018
  
**human\_CMA_motifs** CMA motifs identified in the human proteome 
 
**motif\_modification_reference** (contains information about all possible KFERQ-like motifs) 

**known\_substrates_motivs** CMA motifs identified in known CMA substrates  

**known\_substrates_output_jnet** JPred4 prediction results for the known CMA substrates  

**confirmed_motifs** pdb structres and structure predictions for known CMA substrates  

**one\_canon\_output\_jnet** JPred4 prediction results for proteins with one single canonical motif  

**L2A100_3K.json** (result of the BLAST search for LAMP-2A isoforms)  

**species\_tree\_for_conservation** (taxonomic IDs of the CMA-able and unable species)  

**EggNOG_identifiers.txt** (used to translate from UniProt to EggNOG IDs)  

**newGO\_custom_names.csv** (list of GO terms used for the enrichment analysis)  

**map2slim\_output_tsv.txt** (mapping of child GO terms to the specified parent terms)  

**ratios_list.json** (mapping of the fractional motif content into bins for the triangle plots)  

**conf_motifs** (folder containing structural information for the experimentally confirmed CMA substrates) 

**human_db.csv** (Uniprot reviewed proteins and associated KFERQ-like motif content)

**customGO\_pz\_triangle_groups.txt** (results of GO analysis using the custom GO database for triangle plots)

**customGO\_pz\_reviewed_oneN.txt** (results of GO analysis using the custom GO database for Asparagine-generated motifs)

**human\_compartment\_knowledge_full.tsv** (COMPARTMENTS database downloaded from https://compartments.jensenlab.org/Search)

