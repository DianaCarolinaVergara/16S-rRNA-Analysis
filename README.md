# 16S rRNA Analysis

With this pipeline we can develop a full 16S rRNA analysis with [Qiime2](https://qiime2.org/) (2019.7) (I always worked with hipervariable regions V3-V4) for microbial characterization. After that, with some of these results you can perform the phylosimbiotic and cophylogenetic analysis (for Phylosymbiosis and Co-evolution models).

Better explanaitions in our wiki:
[Wiki](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki)

### You will learn to:


1. Decompress your files `.tar` and Import your sequences `qiime tools import` in Qiime2.
2. Demultiplex `demux`
3. Quality Filter analysis  `qiime dada2 denoise-single` with DADA2.
4. Features table construction 
   > OTUs table
5. Alpha-rarefaction plotting `qiime diversity alpha-rarefaction`
6. Alpha-Beta diversity Analysis
   * Alpha diversity
     > chao1, simpson, shannon, margalef index
   * Beta diversity
    > Bray-Curtis, Weighted, Unweighted-Unifrac
7. Taxonomic classification
8. Construct a phylogeny
9. Classifiers `qiime sample-classifier classify-samples`
   > Random Forest
11. Graphics

    `qiime emperor plot` for Bray-Curtis PCoA
    
    `qiime taxa barplot` for Taxonomic barplots
    
    `time qiime phylogeny fasttree` creating a tree (ML)
    
      or `time qiime phylogeny midpoint-root` for a midpoint rooted tree.
      
    `qiime feature-table heatmap` for heatmaps
10. Export final-files
  > With [Qiime1](http://qiime.org/) 


First, you need to check that you have:
- [X] Installed qiime2 and qiime1 at your HPC cluster
- [X] Load a conda environment `module load anaconda/python3.7`
- [X] Activate qiime2 source `source activate qiime2-2019.7`
- [ ] Preferable start an interactive session or a job.

### References

https://s3-us-west-2.amazonaws.com/qiime2-workshops/fmt-cdiff/index.html#fmt-for-recurrent-clostridium-difficile-infection-tutorial

https://isugenomics.github.io/bioinformatics-workbook/dataAnalysis/Metagenomics/Qiime2.html

http://compbio.ucsd.edu/wp-content/uploads/2018/07/20180621_oslo_university_microbiome_analysis_with_qiime2_tutorial.pdf

https://chmi-sops.github.io/mydoc_qiime2.html

https://forum.qiime2.org/t/q2-phylogeny-community-tutorial/4455
