# Lonestar_Metatranscriptome

# Pipeline is based on the paper "An intuitive guide to processing RNA-seq reads" by Asaduzzaman Prodhan and "ToxCodAn" by Rhett M. Rautsaw
The intention of this pipeline to clean pooled lonestar tick samples, align them to a genome, and identify the most abundant reads for removal. 
Read the paper "Metatranscriptomic investigation of single Ixodes pacificus ticks reveals diverse microbes, viruses, and novel mRNA-like endogenous viral elements" by Calla Martyn et al., for background and future directions behind this pipeline. 

Below I will list each of the software I used in Chronilogical order. Each Software will have a designated folder where you can find example scripts and information on the software. 

-[FastQC](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/) 
Quality check. Run before and after trim

-[Trimgalore](https://github.com/FelixKrueger/TrimGalore) 
Improve reads by removing low quality reads. Dont forget to run Fastqc after

-[HISAT2](https://daehwankimlab.github.io/hisat2/) 
Map the reads back to the referenc genome

-[SAMTools](https://www.htslib.org/) 
Fasta to BAM and SAM files for StringTie

-[FeatureCounts](https://rnnh.github.io/bioinfo-notebook/docs/featureCounts.html)
Will result with counts (which represent how many times the reads map to the genome).

