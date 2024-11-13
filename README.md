# Lonestar_Metatranscriptome
Pipeline for the Lonestar_Metatranscriptome and further anaylsis

#Initial pipeline plan
# Based on the paper "An intuitive guide to processing RNA-seq reads" by Asaduzzaman Prodhan
-[FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/) 
Quality check. Run before and after trim

-[Trimgalore](https://github.com/FelixKrueger/TrimGalore) 
Improve reads by removing low quality reads. Dont forget to run Fastqc after

-[Pear](https://cme.h-its.org/exelixis/web/software/pear/) 
Merge forward and reverse reads together. Can skip this step, but will make life easier in the long run.

-[HISAT2](https://daehwankimlab.github.io/hisat2/) 
Map the reads back to the referenc genome

-[SAMTools](https://www.htslib.org/) 
Fasta to BAM and SAM files for StringTie

-[FeatureCounts](https://rnnh.github.io/bioinfo-notebook/docs/featureCounts.html)
Will result with counts (which represent how many times the reads map to the genome).

