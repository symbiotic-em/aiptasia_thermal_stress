# Aiptasia_thermal_stress_experiment
R scripts and input files for completing analyses described in "Abundance of Oligoflexales bacteria is associated with algal symbiont density independent of thermal stress in Aiptasia anemones", by Emily G Aguirre, Marissa J Fine and Carly D Kenkel. Corresponding author --> emilyagu@usc.edu et al. 

We investigated the role of possible Symbiodiniaceae-associated microbial associates in the holobiont of clonal (aposymbiotic and symbiotic) Aiptasia, strain CC7. 
Anemones were subjected to thermal stress and symbiont expulsion (mild bleaching) was calculated using qPCR. We used amplicon sequencing of the 16S rRNA gene to assess microbial correlations, composition, richness and beta-diversity between anemones in ambient, control conditions vs those in thermally stressed

Annotations in the .R script describe input files, although all analyses can be re-created by starting with the raw .fastq files available for download at NCBI SRA under accession code: PRJNA929535.

# Files in this repository

- Input file: all_oligos.txt text file containing all sequences used for the phylogenetic analyses. Should be connverted to .fa before analysis
- Input file: oligocounts_only_sym.csv count data (total abundance per sample) for oligoflexales in symbiotic anemones only
- Input file: sym1_samdata.csv Metadata for symbiotic anemones only, includes sym host ratios and taxa abundance counts for symbiotic anemones only  
- Input file: samdata_anemone.csv sample data. Metadata including sym host ratios for all  
- Input file: seqtab_anemone.rds sequence table 
- Input file: taxa_anemone.rds taxonomy table

- Sequences: Please see demultiplexed sequences, available at the National Center for Biotechnology Information (NCBI) Sequence Read Archives (SRA) under accession code: PRJNA929535


# Scripts 
- dada2_anemone_16S: Annotated R script (based on DADA2 pipeline tutorial) for making amplicon sequencing variants from fastqc files.
- general_microbiome_analysis: Annotated R script (based on Phyloseq and other statistical software in R) for general analysis and visualization of metabarcoded data
- sym_host_ratio: Annotated R script containing info on how to conduct stats, correlation plots, and visualizations of samples assesed for sym host ratios   

# Statistical output for Metacoder
- output file: metacoder_stat_output.csv statistical output corresponding to differential heat trees created in Metacoder 
- output file: metacoder_taxon_id_key.csv taxon ID keys corresponding to metacoder_stat_output.csv file above 

