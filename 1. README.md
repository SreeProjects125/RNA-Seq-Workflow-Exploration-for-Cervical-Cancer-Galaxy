This workflow turns raw RNA sequencing (RNA-seq) data into a table showing gene activity. 

RNA-seq reads are downloaded from a public database and checked for quality using FastQC, with MultiQC summarizing the results. 

The reads are then aligned to the human reference genome (GRCh38) using RNA STAR. After alignment, featureCounts counts how many reads map to each gene using a gene annotation file. Finally, results from all samples are combined into one clean gene expression dataset that can be used for further analysis.
