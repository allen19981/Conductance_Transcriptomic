# Conductance_Transcriptomic

This is the code for the manuscript "Evaluating Correspondence between Hodgkin-Huxley Computational Neuron Model Ion Channel Conductance and Neuron Type-Specific Transcriptomic Gene Expression"

This notebook has code to download neuronal model ids from the Allen Insititute of Brain Sciences using web scrapping, and analysis tools to plot the processed data gathered. There are two notebooks.

Code_to_download_neuronal_model: This notebook contains the neccessary code to download the neuronal model id to obtain the conductance parameters.

Gene_Conductance_Related_to_Transcriptomic: This notebook contains sections:

- Creating scatterplot comparing gene transcript to conductance parameter
- Calculating spearman correlation and p-value for each correlate
- Ranking spearman correlation for voltage-gated ion channels for each parameter
- Creating histogram to show spread of data for each parameter

# Data

This folder contains 12 file required for plotting and analysis.

all_features.csv: Csv file of all electrophysiology, morphology features, ion conductance, neuronal model id, in one dataframe

all_features_cell_type.csv: Csv file of all electrophysiology, morphology features, ion conductance, neuronal model id, labelled by cell types

transcriptome_df.csv: Transcriptomic gene expression sc-RNAseq data labelled by cell type

sep_layer_df.csv: Transcriptomic gene expressions sc-RNAseq data with all separate cortical layers

new_label_transcriptome_df.csv: Transcriptomic gene expression sc-RNAseq data labelled by cre-line

cre_parameter_df.csv: Relative ion conductance data labelled by cre-lines

abs_parameter_df.csv: Absolute ion conductance data labelled by cell types

sep_layer_cre_parameter_df.csv: Relative conductance data labelled by cell types

entrenz_symbol_s.csv: Csv for entrenz symbol and associated gene

targets_and_families.csv: Csv file about channel genes and their associated ion channels

new_spearman_corr_ranks.json: Spearman Correlation ranks at cre-line level, as a dictionary

sep_spearman_corr_ranks.json: Spearman Correlation ranks for cell types and relative conductance, as a dictionary

abs_spearman_corr_ranks.json: Spearman Correlation ranks for cell types and absolute concductance, as a dictionary
