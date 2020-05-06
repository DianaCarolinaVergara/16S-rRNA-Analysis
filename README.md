# 16S rRNA Analysis

With this pipeline we can develop a full 16S rRNA analysis with [Qiime2](https://qiime2.org/) (2019.7) (I always worked with hipervariable regions V3-V4) for microbial characterization. After that, with some of these results you can perform the phylosimbiotic and cophylogenetic analysis (for Phylosymbiosis and Co-evolution models).

Better explanaitions in our wiki:
[Wiki](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki)



![qiime2](https://qiime2.org/assets/img/qiime2.svg)

.

.


### You will learn to:


1. Why 16S [rRNA](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/1.-Why-16S-rRNA)?

![](https://camo.githubusercontent.com/8125565a1073969bccf54ea0f82d689d522ee08f/68747470733a2f2f68656c702e657a62696f636c6f75642e6e65742f77702f77702d636f6e74656e742f75706c6f6164732f323031372f30352f3136735f7661725f726567696f6e2e706e67)

2. Decompress your [files](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/2.-Decompress-files) `.tar` and Import your sequences `qiime tools import` in Qiime2.

3. Import Data & Demultiplex `demux` [files](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/3.-Import-Data-&-Demultiplex)

![](https://camo.githubusercontent.com/955eb5fa960831ac8c3a97343c9954e0d2a322b0/68747470733a2f2f7777772e7265736561726368676174652e6e65742f70726f66696c652f4368756e5f4a696d6d69655f59652f7075626c69636174696f6e2f3332313733353038372f6669677572652f666967312f41533a36333636343037333733373031313240313532383739383338383739342f44656d75786c65742d64656d756c7469706c6578696e672d616e642d646f75626c65742d6964656e74696669636174696f6e2d66726f6d2d73696e676c652d63656c6c2d646174612d612d506970656c696e652d666f725f573634302e6a7067)

4. Quality [Filter analysis](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/4.-Quality-Filter)  `qiime dada2 denoise-single` with DADA2.


5. Features table [construction](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/5.-Feature-Table-Construction) 
   > OTUs table
6. Alpha-rarefaction [plotting](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/5.-Feature-Table-Construction) `qiime diversity alpha-rarefaction`
7. Alpha-Beta diversity Analysis
   * [Alpha diversity](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/8.1.-Alpha--Diversity-Analysis)
     > chao1, simpson, shannon, margalef index
   * [Beta diversity](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/8.2-Beta-Analysis)
    > Bray-Curtis, Weighted, Unweighted-Unifrac
    
    
    ![](https://camo.githubusercontent.com/3778262e8c516adfcfb5048a1c3ab0ae4d9ccffa/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f7468756d622f372f37332f426574615f76735f6c617469747564652e6769662f33333070782d426574615f76735f6c617469747564652e676966)
    ![](https://camo.githubusercontent.com/c12c95aa9d8d938275ba97944f2bb5367d5c4a0b/68747470733a2f2f6472697665352e636f6d2f757365617263682f6d616e75616c2f6f74755f7461626c652e6a7067)
    
8. Taxonomic classification [(assignation)](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/9.-Taxonomic-Classification)

9. Construct a phylogeny
   > [Phylogenetic Analysis](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/10.-Construct-a-Phylogeny)
   
10. Classifiers `qiime sample-classifier classify-samples`
   > [Random Forest](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/11.-Classifiers)
   
   ![](https://camo.githubusercontent.com/8c5317ce22acf5661a37eab0009be8c29f24dfe1/68747470733a2f2f6472697665352e636f6d2f757365617263682f6d616e75616c2f636c61737369666965722e676966)
   
11. Graphics
   
   > [Plotting graphics](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/12.-Graphics)
   
   - PCoA
   
        `qiime emperor plot for Bray-Curtis PCoA`
    
   - Taxonomic Baplots
    
        `qiime taxa barplot` 
    
   - Trees
    
        `time qiime phylogeny fasttree` creating a tree (ML)
    
      or `time qiime phylogeny midpoint-root` for a midpoint rooted tree.
      
   - Heatmaps
      
        `qiime feature-table heatmap` for heatmaps
    
   
 ![](https://camo.githubusercontent.com/9cafaae7b8b19f5390b3e860bea01ba21b77f77f/68747470733a2f2f666f72756d2d7169696d65322d6f72672e73332e6475616c737461636b2e75732d776573742d322e616d617a6f6e6177732e636f6d2f6f726967696e616c2f32582f632f636665333436616464653161633962373239326461613862643835636661623562383434623361322e676966)
  
  
12. Export final-[files](https://github.com/DianaCarolinaVergara/16S-rRNA-Analysis/wiki/13.-Export-Files)
  > With [Qiime1](http://qiime.org/) 
  
  
  ![](https://camo.githubusercontent.com/e52928fe0a62e4db03fe3c82b4bf55c95e5fcd2a/687474703a2f2f7169696d652e6f72672f686f6d655f7374617469632f696d616765732f7169696d655f6c6f676f5f6c617267652e706e67)
  ![](https://camo.githubusercontent.com/59590379634ff33ddac6945f6365f424b208fd2b/687474703a2f2f62696f6d2d666f726d61742e6f72672f5f696d616765732f62696f6d2d666f726d61742e706e67)
.
.

First, you need to check that you have:
- [X] Installed qiime2 and qiime1 at your HPC cluster
- [X] Load a conda environment `module load anaconda/python3.7`
- [X] Activate qiime2 source `source activate qiime2-2019.7`
- [ ] Preferable start an interactive session or a job.

.

![](https://qiime2.org/assets/img/q2cli.png)

.


### References

- https://s3-us-west-2.amazonaws.com/qiime2-workshops/fmt-cdiff/index.html#fmt-for-recurrent-clostridium-difficile-infection-tutorial

- https://isugenomics.github.io/bioinformatics-workbook/dataAnalysis/Metagenomics/Qiime2.html

- http://compbio.ucsd.edu/wp-content/uploads/2018/07/20180621_oslo_university_microbiome_analysis_with_qiime2_tutorial.pdf

- https://chmi-sops.github.io/mydoc_qiime2.html

- https://forum.qiime2.org/t/q2-phylogeny-community-tutorial/4455

.

.

.
## The End...?

Phylosymbiosis and Coevolution Analyses

Next:

- [X] SNPs Analysis [Pipeline](https://github.com/DianaCarolinaVergara/SNPs_pipeline)
- [X] Host Phylogeny 
- [ ] Phylosymbiosis
- [ ] Coevolution

![](https://camo.githubusercontent.com/d4032f16242baa159607e5a9c797359675ccde75/68747470733a2f2f692e70696e696d672e636f6d2f323336782f35302f34392f32342f35303439323435353263643939626361396432623231666437633839326365382d2d636f72616c2d626c65616368696e672d6f6365616e2d70686f746f732e6a7067)
![](https://camo.githubusercontent.com/d6043736b6c0c076026ad55de9d07e9464ec58e5/68747470733a2f2f692e70696e696d672e636f6d2f323336782f30662f33322f39342f30663332393438313238383461613733353830383030663330376332623762662d2d636f72616c2d72656566732d617175617269756d732e6a7067)
