# Filtered_MSA_SARS_CoV_2
There is one .pdf file and 3 file folds included. 
Each fold for a genome sequences data-set collected from GISAID database till the date indicated by the folder name.
There are 6 files included in each folder. One .png file,  one .xls file and four .mat files. 
The .png file shows the top 100 significant pairwise PLM scores. The links beween/to the non-coding region are discarded in the circos plot. The greys for the links with PLM scores located in top 51 to 100. The red and blue are for top 50s while red for close links (the distance between loci is less than 4), blue for far links.
The .xls file presents the rank, protein, type of mutations for each terminal of pairwise links as well as the indice of locus in the reference sequence "Wuhan-Hu-1" (https://www.ncbi.nlm.nih.gov/nuccore/MN908947).
Other .mat files are full header files, filtered headers, filtered and mapped MSA files ('-NACGT' ---> '012345') , remainning loci indices with respect to the reference sequences respectively.


---------------------
updated on 2021-12-22

1. The Accession IDs for the genomic sequences we used in the analysis are divided into two parts as the limitation of file size. One is name as "Dataset1-1-Mar-2020-May-2021-Accession_IDs.xlsx" and the other one named as "Dataset1-1-Jun-2021-Oct-2021-Accession_IDs.xlsx". The prefix of each sequence "EPI\_ISL\_" is excluded to decrease the file size.


2. Dataset2-p0.98_plm_Top200_No_3variants.xlsx  contains selected links in top 200 plmDCA epistasic pairs, as ranked by their score. The plmDCA links shown in Fig. 3 in the main text are based on this dataset. Here, the links located in the non-coding region and with close locus ($\le 5$) and any loci included in alpha, beta, delta are excluded.


3. Dataset3-p0.98_Top_2000_CA_No_variants.xlsx lists the sorted correlation scores. Similarly to its plm counterpart, links in coding region and the distance between loci is larger than 5bps are considered. No variants are included.

4. Dataset4-links_with_Spike_locus_or_loci_ranks.xlsx}{The epistasis provided by plmDCA and correlation analysis are included in this dataset for each month. Only those within top-200s, for which the distance between two terminals is $\gt 5$ loci and whose both terminals located in the coding region are listed in the dataset. 

5. Dataset5-protein_aa_mut_for_links_in_Dataset4.xlsx provides the links within top 200s plmDCA scores that containing Spike terminals, for each month. The short links with loci located within 5 bps are discarded. Here, we also annotate the genes to which loci in the Dataset4 belong to and the corresponding amino acid mutations. The annotated genes and corresponding amino acid mutations in Table 1 and 2 in the main body of the manuscript are based on this dataset.
