# [Bankers, et al 2017](https://onlinelibrary.wiley.com/doi/epdf/10.1111/mec.14146) 

Bankers, L, Fields, P, McElroy, KE, Boore, JL, Logsdon, JM, Neiman, M. Genomic evidence for population‐specific responses to co‐evolving parasites in a New Zealand freshwater snail.  

Mol Ecol. 2017; 26: 3663– 3675. https://doi.org/10.1111/mec.14146 

 

# 0. GitHub  

https://github.com/Intro-Sci-Comp-UIowa/biol-4386-course-project-cmhggns 

  

# 1. Introduction 

Scientists have been baffled for years by the mystery of sex. Sexual organisms have high genetic diversity due to genetic exchange in reproduction, but it is much more taxing than asexual reproduction, or many of the other alternative forms of reproduction. In contrast, asexual reproduction is an exponential, more efficient method of reproduction, but it comes with the accumulation of mutations, good and bad, and a relative lack of genetic variation. The so called “Mystery of Sex” is primarily about why sexual reproduction persists, given its costly nature, but it is also worthwhile to ask how asexual populations can persist and evolve. 

The Potamopyrgus antipodarum, or New Zealand Mud Snail, is a mollusc native to New Zealand, and invasive to almost every continent. This incredible snail can be either sexual or asexual, with varying levels of ploidy, so it is an excellent model organism for studying the differences between and evolution of sexual and asexual reproduction.  

It has been widely hypothesized that asexual populations maintain variation through high ploidy levels and rapid evolution. P. antipodarum has varying levels of ploidy, primarily between diploid and tetraploid, which may be how it is able to maintain a moderate level of genetic variation within populations. P. antipodarum also undergoes rapid evolution caused by host-parasite interactions. 

Host-parasite interactions are one of the primary sources of natural selection and are a powerful fool for studying evolutionary responses to strong selection. Antagonistic coevolution between host and parasite, like the host-parasite interactions within P. antipodarum, can maintain high genetic diversity and drive rapid diversification. These interactions have been highly characterized in plants and their pathogens, but there is a lack of knowledge in how these interactions can affect populations of animals in nature. In many studies, host-parasite interactions have been implicated in genetics, rapid molecular coevolution, and changes genetic expression, but a majority of these studies have been performed in laboratory settings with bred model organisms. (Abbate, et al 2015, Hamilton 1980, Bérénos, et al 2011, van Houte, et al 2016, King, et al 2011a, 2011b, Laine, 2009, Masri, et al 2015, Paterson, et al 2010) 

One of the most common parasites of the P. antipodarum is the Microphallus sp. (Microphallus), which uses it as an intermediate host. The Microphallus will infect the snail, completely sterilizing it, and the snail will then be eaten by one of its higher predators, such as the dabbling duck (Anatinae). Once the dabbling duck has eaten the infected snail, the Microphallus will infect the dabbling duck as its final host, completing its lifecycle. While infected, the dabbling duck will continue its migration across New Zealand, spreading the microphallus and increasing gene flow.  (Bankers, 2017)

By studying the interactions between P. antipodarum and Microphallus, we aim to classify genomic evidence of antagonistic evolution. To do this, we will use RNA-seq gene expression analyses and FST analyses to study uninfected P. antipodarum and those at a stage V infection status in three separate lake populations. Through our review of existing ecological studies on local adaption and coevolution, we expect to see some difference between populations in gene expression trends, varying by infection status and lake of origin. In this study, we hope to use the genomic variation between infected and uninfected snails in different lakes to classify coevolution in real time, further our understanding of these antagonistic adaptive interactions, and provide valuable knowledge for ecology experts across the globe who are interested in how these host-parasite interactions may affect their local wildlife.  

 

![N|Solid](https://onlinelibrary.wiley.com/cms/asset/a8e764af-bab5-4fd6-b0c5-89c880344feb/mec14146-fig-0001-m.jpg) 

 

> **Figure 1.** *"Heatmaps representing significantly differentially expressed transcripts (higher FPKM = higher expression). Significance was assessed with a FDR of 5% and Benjamini‐Hochberg multiple test correction. (a) Inclusive analysis: 1,408 significantly differentially expressed transcripts in infected vs. uninfected snails. Transcripts above the black line demarcated with asterisks are downregulated in infected snails (1,057), and transcripts below this line are upregulated in infected snails (351). (b) Within‐lake analysis: dendrogram and heatmap representing the 6,228 significantly differentially expressed transcripts across infection status and lakes. “Ax” = Alexandrina, “Se” = Selfe, “Kn” = Kaniere, red = infected, blue = uninfected. Snails clustered by lake of origin rather than infection status, indicating spatially structured gene expression patterns. Highlighted regions of heatmap contain examples of: expression differences between infected and uninfected snails within a lake (green), lake‐specific expression regardless of infection status (downregulation in Ax, blue) and across‐lake upregulation in infected snails (purple)"(Bankers 2017)* 

 

Upon the conclusion of the original study performed by Bankers, et al in 2017, the authors found that there was a systematic reduction of gene expression among infected P. antipodarum, with their results plotted in a heat map in Figure 1. The authors found that of the 62,862 transcripts present in the de novo reference transcriptome, 1,408 transcripts were significantly differentially expressed between the infection statuses, with an FDR of 5%, Benjamini-Hochberg multiple test correction, seen in figure 1a. Approximately 75% of these differentially expressed transcripts were downregulated in the infected snails (Fisher’s exact test, p<0.0001), shown in figure 1a. There were 373 transcripts with an FPKM of 4 or higher and a two-fold difference in expression, with 349 of those being downregulated. The authors then concluded that P. antipodarum, when infected, experience global gene expression reduction, and they went on to do a functional analysis, discussed in the Results section, below. (Bankers, 2017)

 

# 2. Methods 

### 2.1 Sample collection, dissection, and selection 

 This study uses adult, diploid, female P. antipodarum that are non-brooding. Adult snails were collected from the lake shores of Lake Alexandrine, Lake Kaniere, and Lake Selfe in New Zealand using insect collection nets. Upon arrival to the University of Iowa, the snails were housed in conditions replicating that of the lakes of New Zealand (16C water, 16:8 light:dark cycles to simulate a circadian rhythm, and dried spirulina to eat) for one week. (Bankers, 2017)

Upon recovery from international trial, the snails were ready for dissection and RNA isolation. P. antipodarum can be sexual or asexual with varying levels of ploidy, so RNA-seq analysis was only conducted on diploid adult nonbrooding (not actively reproducing) females to ensure minimal confounding effects, such as biological processes related to reproduction, would not be conflated with differences in expression due to the host-parasite interactions we aim to study. The snails were each dissected and classified by sex (male/female), infection status (stage 5 infection/uninfected), and reproductive status (brooding/nonbrooding). Microphallus infection fills the entire body cavity, so RNA-seq must be confined to head tissue. (Bankers, 2017)

The acquired head tissue from each snail was split in half for separate analyses. Half of the tissue from each sample was stored for later RNA extraction using RNAlater (Life Technologies Corporation), while the other half was immediately snap frozen in liquid nitrogen and used for flow cytometry. Genome size, and thus ploidy, was estimated through flow cytometry of the head tissue using the protocol outlined in Krist, Kay, Larkin, and Neiman (2014). RNA was extracted from the tissue via the Invitrogen TRIzol protocol (Chomcynski, 1993), and RNA quality/quantity were estimated using a Bio-Rad Experion Automated Electrophoresis Station, via the manufacturer protocol of the Experion RNA analysis kit. For each replicate used for RNA-seq, head tissue was pooled from seven snails with the same lake and infection status. Three of each of these replicates were obtained, for a total of 18 replicates and 126 snails. (Bankers, 2017)

### 2.2 RNA Sequencing and de novo transcriptome assembly and annotation 

Upon extraction of the RNA, RNA shearing and cDNA library preparation were done following the Illumina Truseq RNA Sample Prep v2 LS protocol (Illumina, San Diego, CA, 2012). Illumina HiSeq 2000 was used for 2 x 100 bp paired-end RNA-seq. Every sample of RNA was given a unique adapter sequence (Illumina, 2012) and was separated into two halves, each of which were sequenced separately. The mean read length was 100.7 base pairs (standard deviation = 0.96bp), and the mean number of paired-end reads per replicate per lane was 10,070,420 (standard deviation = 1,474,539.1) for 20,000,000 paired-end reads per replicate. FASTX Toolkit (Gordon and Hannon, 2010) and FastQC (Andrews, 2010) were used to trim the added adapter sequences, assess sequence quality, and remove low-quality reads. The mean sequence quality (Phred) score was 35.95, and the mean number of reads/replicate/lane was 9,871,440.4 (standard deviation = 1,468,645.04) for 18,000,000 paired-end reads per replicate.  (Bankers, 2017)

Trinity version 2.0.4 (Grabherr et al., 2011, Haas et al., 2013) was then used to generate a de novo transcriptome assembly, following the protocol given by Grabherr et al (2011) and Haas et al (2013). Trinity in silico normalization was performed for each replicate to maximize the representative read set while reducing required memory for the assembly process. The reads were then normalized into a preliminary transcriptome assembly, using Haas, et al (2013). Protein-coding regions in the transcriptome were annotated using the TransDecoder trinity plugin (Haas, et al 2013), which identified long open reading frames, retained the longest open reading frame of a predicted coding sequence, and filtered out miscalled isoforms. Hierarchal clustering was used based on sequence identity, as outlined in CD-HIT-EST (Huang, et al 2010). Potential contaminants were identified and eliminated using the blobology pipeline script “blast_taxonomy_report.pl” (Kumar, et al 2013), blastx (Camacho, et al 2009), and a custom pipeline created by Joal Sharbrough (github.com/jsharbrough/grabContigs). Blobology was used to identify the top blastx hits, and the transcripts found to be Non metazoan taxa or Platyhelminthes through blastx analysis were removed. The resulting transcriptome was annotated using blastx (Camacho, et al 2009) with an E-value of 1e-5. Blast2go (Conesa, et al 2005) and pfam (Finn, et al 2016) were used to assign gene ontology terms to the resulting assembly. (Bankers, 2017)

### 2.3 RNA-seq gene expression analysis 

Tophat2 (Trapnell, et al 2013) was used to map the RNA-seq reads to the de novo reference transcriptome. Mapped reads were then assembled into transcripts and transcript abundance was estimated through cufflinks (Trapnell, et al 2010). Cufflinks GTF and Tophat bam files were merged via Cuffmerge (Trapnell, et al 2012), which was then used to identify significant gene expression changes in CuffDiff (Trapnell, et al 2012), with an FDR of 5% and a Benjamini-Hochberg multiple test correction. A parameter that was set was the transcripts must exceed 0 fragments per kilobase per million reads mapped (FPKM) to ensure the genes were transcribed in all replicates. Transcripts with >4 FPKM and a twofold difference in gene expression across infection status were isolated to identify differentially expressed genes that were the most relevant. The results of this analysis were visualized in heatmaps and a dendrogram, made by cummeRbund (Goff, et al 2013). (Bankers, 2017)

### 2.4 Recreation of Figure 1 

In the recreation of the heatmaps and dendrogram shown in Figure 1, generated by cummeRbund (Goff, et al 2013), we used the CuffDiff output files, obtained from Laura Bankers (https://github.com/Intro-Sci-Comp-UIowa/biol-4386-course-project-cmhggns/tree/main/code/biol-4386-course-project-cmhggns/data). These output files were analyzed using CuffDiff (Trapnell, et al 2012) again to quantify the number of differentially expressed genes and identify any significant changes in expression. We then used cummeRbund (Goff, et al 2013) to create the dendrogram and heatmap for each file. Upon the plots being generated, they were added to a PowerPoint, version 2103 (Microsoft Corporation, Redmond, WA, 2021) for resizing, labeling, and superimposing lines to separate columns. 

The full annotated de novo transcriptome assembly is available on GitHub (https://github.com/Intro-Sci-Comp-UIowa/biol-4386-course-project-cmhggns/tree/main/data) 

 

# 3. Results and Discussion 

### 3.1 Results 

The initial transcriptome assembly, created through Trinity, contained 462,736 transcripts, and after filtering with TransDecoder, CD-HIT-EST, and Blobology, the final transcriptome assembly contained 62,862 transcripts, 39,557 of which were annotated using BLASTX, blast2go, and pfam. The 37.1% of the transcriptome that wasn’t annotated is not surprising, given the lack of external mollusc genome sequence data (Kocot, et al 2015). Of the 62,862 transcripts in the assembly, 1,408 were significantly differentially expressed across infection status, with an FDR of 5% and a Benjamini-Hochberg multiple test correction, Figure 1a, 2a. 1,057 of the significantly differentially expressed transcripts were downregulated in the infected snails (Fisher’s exact test: p<0.0001), Figure 1a. 373 of those transcripts had an FPKM of at least 4 and a twofold difference in expression between infected and uninfected snails; 349 of which were downregulated. Given this data, it is fair to conclude that P. antipodarum that are at a stage 5 Microphallus infection experience a systematic reduction of gene expression. (Bankers, 2017)

  

![N|Solid](https://raw.githubusercontent.com/Intro-Sci-Comp-UIowa/biol-4386-course-project-cmhggns/main/figures/modified_final_figures.jpg) 

> **Figure 2** *Figure 2 is a recreation of Figure 1 from Bankers, et al 2017. These heatmaps show significantly differentially expressed transcripts on a logarithmic scale of frames per kilobase per million reads (FPKM), with higher FPKM values showing higher expression. Figure 2a shows an inclusive analysis, where all snails with a stage 5 microphallus infection are analyzed together, regardless of lake of origin. This heatmap shows 1,408 significantly differentially expressed transcripts between infection classes, 1,057 of which were downregulated in infected snails. Figure 2b shows a similar analysis, broken down also by lake of origin, with a heatmap and a dendrogram to show diversification between lake populations. Trends within 2b show spatially structured gene expression. Lake designation: Ax = Alexandrina, Se = Selfe, Kn = Kaniere, Infection designation: red = infected, blue = uninfected.* 

 

After the inclusive analysis, another analysis was done, breaking the snails down by lake of origin, Figure 1b, 2b. Bankers, et al (2017) found that within each lake, in the 62,862 transcripts, 1,534 transcripts were significantly differentially expressed across infection statuses, and 610 of them had at least 4 FPKM and a twofold difference in gene expression. When comparing across each lake, the authors found 6,228 significantly differentially expressed transcripts that differ within and across lake of origin, 75% of which were significantly differentially expressed, regardless of infection status. This shows that the lake the snail originated from has a stronger influence on gene expression than infection status, Figure 1b, 2b. (Bankers, 2017)

### 3.2 Discussion 

Figure 2 is a close replication of Figure 1, but there are a few differences between the two. Figure 1a shows a line of significance, breaking up the downregulated transcripts in the infected snails, but this is not included in Figure 2a because of a lack of statistical test and the possibility of excess genes. Though the original author and I used the same CuffDiff output files and commands within CuffDiff and cummeRbund, I hypothesize that there may be differences in our data. R has been updated since the original analysis was done in 2016/2017, so I believe that there may be a slight difference in coloring, causing a slight visual difference in coloring between Figures 1 and 2. Additionally, there seems to be additional genes being represented in Figure 2, most strikingly in Figure 2a, where there seems to be highly expressed transcripts in the uninfected snails, below where the line of statistical significance would have been, had it been included. This difference in gene representation could have due to the transcripts in my transcriptome being in a slightly different order, the difference in operating system, a difference in files used to create the figure, or a masking effect, caused by the placement of the statistical significance line. I did not include the line of statistical significance because I did not perform Fisher’s exact test on this data set, and thus couldn’t accurately place the line.  

Seeing Figure 2a as a heat map without superimposed lines of significance highlight the possible difference in represented transcripts, which visually may not be significantly differentially expressed. It is possible that in the original figure, these transcripts were not classified as significantly differentially expressed, so they were excluded from the analysis. According to Bankers, et al (2017), Figure 1a was generated using the 1,408 significantly differentially expressed transcripts, and while Figure 2a was performed on the CuffDiff output files, CuffDiff automatically finds the data, meaning it could have redone the analysis on an earlier, unfiltered transcriptome file, housed within the output file that was given to me. Another possibility is simpler: the assembly and R could have changed enough in the past 5 years to cause this difference visually, affecting the coloring or order of the transcriptome, but not the data itself. 

Another difference is that Figure 2b does not include the colored boxes that are used in Figure 1b to show trends. I did not include these because I wasn’t sure if the original author put these boxes in very precise places, based on a mathematical approach, so because I could not replicate exactly where the author put them, I did not add them. If I had attempted to place these boxes in the exact same places, I would have shown different trends than intended, due to the different in transcript placement or amount, as discussed above. 

 

# 4. Conclusion 

Regardless of the differences between figures, the conclusion is the same. Through the significant gene expression feature in CuffDiff, both the original author’s and my calculations result in 373 significantly differentially expressed transcripts with a FPKM of 4 or greater and a twofold difference in expression between classes. In both cases, this leads to the conclusion that infected P. antipodarum have a global downregulation in expression, compared to their uninfected counterparts. 

The original authors go on to use the total transcripts identified as significantly differentially expressed across infection status within at least one of the lakes, as shown in Figure 1b, 2b), to compare significant differences between single and multiple populations. By doing this separate analysis, they were able to determine if snails from each lake have different responses to Microphallus infection, or if it is shared across all lakes studied. 94% of the transcripts were only expressed in a single lake, showing that there are lake-specific (local) responses in gene expression to parasite infection. This finding supports the population genetic structure in gene expression, as discussed in Neiman, et al (2004, 2011) and Paczesniak, et al (2013) in P. antipodarum. (Bankers, 2017)

 

# 5. Reflection 

### 5.1 Barriers to Reproducibility 

There were several barriers to reproducibility that I would like to discuss. In my quest to understand and use CuffDiff and cummeRbund, I ran into several issues and had to research possible solutions online. While doing this, I found a surprising lack of up-to-date documentation or current corresponding authors. Often, people create programs to analyze their own data, and make them available for everyone to use. When their experiment is over, they often leave their program as it is, not spending any extra time or effort on keeping it updated. I have seen this happen in my own lab as well. Because our organism is not widely studied, we create a lot of our own code, pipelines, and programs, and while we do improve it, we did not have an updated GitHub until last month. When we are done using a pipeline, etc., like the one Joel created, mentioned in the methods section, we tend to just move on, without worrying about maintaining it. Because of the relative lack of popularity and maintenance of my programs, it is no wonder that there is a lack of documentation, online discussion, and updates. 

Another issue with reproducibility would be the figure modification. I followed the instructions from the original author exactly, but mine still looked different. It was clear that she had resized the figure and added labels, lines, and boxes, so I did as well. As I was doing this, I realized how easy it would be to show a misleading message, just by making certain lines thicker, adding a box, or isolating a specific region of a plot. I didn’t modify any data points, but when I changed the proportions of the plot and added thick lines on top, it was easy to minimize areas that weren’t aligned with my message, most likely without my reader catching on. This is a major issue, both with reproducibility and academic integrity. 

In response to some of the issues my classmates and I faced, I have started keeping a better digital notebook with the exact code I tried and the results. I have also been working on my file structure, and I convinced my lab to create a public GitHub. Prior to this, all of our data was stored in separate locations, and we actually used slack for a lot of file sharing. For me, this was fine, until the people in charge of slack decided to switch plans, and I got kicked out. Once I was accidentally removed from the group, I realized how difficult it is to find any of the data needed to reproduce results from our research group. Even if no one outside of our research group will use the GitHub, having it is actually cheaper and more sustainable for the lab because we don’t need to pay extra for each person that views our data, and it won’t be deleted if we decide to stop paying for our large group Slack. 



------
# References: 

Abbate, J., Kada, S., & Lion, S. (2015). Beyond mortality: Sterility as a neglected component of parasite virulence. PLoS Pathogens, 11, 1– 10. https://doi.org/10.1371/journal.ppat.1005229 

Adema, C. M., Hanington, P. C., Lun, C. M., Rosenberg, G. H., Aragon, A. D., Stout, B. A., … Loker, E. S. (2010). Differential transcriptomic responses of Biomphalaria glabrata (Gastropoda, Mollusca) to bacteria and metazoan parasites, Schistosoma mansoni and Echinostoma paraensei (Digenea, Platyhelminthes). Molecular Immunology, 47, 849– 860. https://doi.org/10.1016/j.molimm.2009.10.019 

Adema, C. M., & Loker, E. S. (2015). Digenean‐gastropod host associations inform on aspects of specific immunity in snails. Developmental and Comparative Immunology, 48, 275– 283. https://doi.org/10.1016/j.dci.2014.06.014 

Andrews, S. (2010). FastQC: A quality control tool for high throughput sequence data. Available: http://www.bioinformatics.babraham.ac.uk?/projects/fastqc/ 

Arican‐Goktas, H. D., Ittiprasert, W., Bridger, J. M., & Knight, M. (2014). Differential spatial repositioning of activated genes in Biomphalaria glabrata snails infected with Schistosoma mansoni. PLoS Neglected Tropical Diseases, 8, 1– 10. https://doi.org/10.1371/journal.pntd.0003013 

Bankers, L, Fields, P, McElroy, KE, Boore, JL, Logsdon, JM, Neiman, M. Genomic evidence for population‐specific responses to co‐evolving parasites in a New Zealand freshwater snail. Mol Ecol. 2017; 26: 3663– 3675. https://doi.org/10.1111/mec.14146 

Barribeau, S. M., Sadd, B. M., du Plessis, L., & Schmid‐Hempel, P. (2014). Gene expression differences underlying genotype‐by‐genotype specificity in a host‐parasite system. Proceeding of the National Academy of Sciences USA, 111, 3496– 3501. https://doi.org/10.1073/pnas.1318628111 

Bérénos, C., Wegner, K. M., & Schmid‐Hempel, P. (2011). Antagonistic coevolution with parasites maintains host genetic diversity: An experimental test. Proceedings of the Royal Society of London B, 27, 218– 224. https://doi.org/10.1098/rspb.2010.1211 

Bergstrom, C. T., & Dugatkin, L. A. (2016). Evolution, 2nd ed. New York: W. W. Norton and Company. 

Brunner, F. S., Schmid‐Hempel, P., & Barribeau, S. M. (2013). Immune gene expression in Bombus terrestris: Signatures of infection despite strong variation among populations, colonies, and sister workers. PLoS ONE, 8(7), 1– 9. https://doi.org/10.1371/journal.pone.0068181 

Camacho, C., Coulouris, G., Avagyan, V., Ma, N., Papadopoulos, J., Bealer, K., & Madden, T. L. (2009). BLAST+: Architecture and applications. BMC Bioinformatics, 10, 1– 9. https://doi.org/10.1186/1471-2105-10-421 

Chomczynski, P. (1993). A reagent for the single‐step simultaneous isolation of RNA, DNA, and proteins from cell and tissue samples. BioTechniques, 15(532–534), 536– 537. 

Conesa, A., Götz, S., García‐Gómez, J. M., Terol, J., Talón, M., & Robles, M. (2005). Blast2GO: A universal tool for annotation, visualization and analysis in functional genomics research. Bioinformatics, 21, 3674– 3676. https://doi.org/10.1093/bioinformatics/bti610 

Coustau, C., Gourbal, B., Duval, D., Yoshino, T. P., Adema, C. M., & Mitta, G. (2015). Advances in gastropod immunity from the study of the interaction between the snail Biomphalaria glabrata and its parasites: A review of research progress over the last decade. Fish and Shellfish Immunology, 4, 5– 16. https://doi.org/10.1016/j.fsi.2015.01.036 

Decaestecker, E., Gaba, S., Raeymaekers, J. A. M., Stoks, R., Van Kerckhoven, L., Ebert, D., & De Meester, L. (2007). Host‐parasite ‘Red Queen’ dynamics archived in pond sediment. Nature, 450, 870– 873. https://doi.org/10.1038/nature06291 Decaestecker, E., Gaba, S., Raeymaekers, J. A. M., Stoks, R., Van Kerckhoven, L., Ebert, D., & De Meester, L. (2007). Host‐parasite ‘Red Queen’ dynamics archived in pond sediment. Nature, 450, 870– 873. https://doi.org/10.1038/nature06291 

De Wit, P., Pespeni, M. H., & Palumbi, S. R. (2015). SNP genotyping and population genomics from expressed sequences ‐ current advances and future possibilities. Molecular Ecology, 24, 2310– 2323. 

Dybdahl, M. F., & Krist, A. C. (2004). Genotypic vs. condition effects on parasite‐driven rare advantage. Journal of Evolutionary Biology, 17, 967– 973. https://doi.org/10.1111/j.1420-9101.2004.00759.x 

Finn, R. D., Coggill, P., Eberhardt, R. Y., Eddy, S. R., Mistry, J., Mitchell, A. L., … Bateman, A. (2016). The Pfam protein families database: Towards a more sustainable future. Nucleic Acids Research, 44, D279– D285. https://doi.org/10.1093/nar/gkv1344 

Gleichsner, A. M., Thiele, E. A., & Minchella, D. J. (2015). It's all about those bases: The need for incorporating parasite genetic heterogeneity into the development of schistosome vaccines. PLoS Neglected Tropical Diseases, 9, 1– 5. https://doi.org/10.1371/journal.pntd.0003805 

Goff, L., Trapnell, C., & Kelley, D. (2013). cummeRbund: Analysis, exploration, manipulation, and visualization of Cufflinks high‐throughput sequencing data. R Package v. 2.12.0. 

Gordon, A., & Hannon, G. (2010). Fastx‐toolkit. FASTQ/A short‐read pre‐processing tools (unpublished). http://hannonlabcshledu/fastx_toolkit/ 

Grabherr, M. G., Haas, B. J., Yassour, M., Levin, J. Z., Thompson, D. A., Amit, I., … Regev, A. (2011). Full‐length transcriptome assembly from RNA‐Seq data without a reference genome. Nature Biotechnology, 29, 644– 652. https://doi.org/10.1038/nbt.1883 

Haas, B. J., Papanicolaou, A., Yassour, M., Grabherr, M., Blood, P. D., Bowden, J., … Regev, A. (2013). De novo transcript sequence reconstruction from RNA‐seq, using the Trinity platform for reference generation and analysis. Nature Protocols, 8, 1494– 1512. https://doi.org/10.1038/nprot.2013.084 

Hamilton, W. D. (1980). Sex versus non‐sex versus parasite. Oikos, 35, 282– 290. https://doi.org/10.2307/3544435 

Herron, J. C., & Freeman, S. (2014). Evolutionary analysis, 5th ed. Glenview, IL: Pearson Education, Inc. 

Holomuzki, J. R., & Biggs, B. J. F. (2006). Habitat‐specific variation and performance trade‐offs in shell armature of New Zealand mudsnails. Ecology, 87, 1038– 1047. https://doi.org/10.1890/0012-9658(2006)87[1038:HVAPTI]2.0.CO;2 

Jokela, J., Dybdahl, M. F., & Lively, C. M. (2009). The maintenance of sex, clonal dynamics, and host‐parasite coevolution in a mixed population of sexual and asexual snails. American Naturalist, 174, S43– S53. https://doi.org/10.1086/599080 

Jurberg, A. D., & Brindley, P. J. (2015). Gene function in schistosomes: Recent advances toward a cure. Frontiers in Genetics, 6, 1– 4. https://doi.org/10.3389/fgene.2015.00144 

King, K. C., Jokela, J., & Lively, C. M. (2011a). Parasites, sex, and clonal diversity in natural snail populations. Evolution, 65, 1474– 1481. https://doi.org/10.1111/j.1558-5646.2010.01215.x 

King, K. C., Jokela, J., & Lively, C. M. (2011b). Trematode parasites infect or die in snail hosts. Biology Letters, 7, 265– 268. https://doi.org/10.1098/rsbl.2010.0857 

King, K. C., & Lively, C. M. (2009). Geographic variation in sterilizing parasite species and the Red Queen. Oikos, 118, 1416– 1420. https://doi.org/10.1111/j.1600-0706.2009.17476.x 

Kofler, R., Pandey, R. V., & Schlötterer, C. (2011). Popoolation 2: Identifying differentiation between populations using sequencing of pooled DNA samples (Pool‐Seq). Bioinformatics, 27, 3435– 3436. https://doi.org/10.1093/bioinformatics/btr589 

Konczal, M., Koteja, P., Stuglik, M. T., Radwan, J., & Babik, W. (2014). Accuracy  

Krist, A. C., Kay, A. D., Larkin, K., & Neiman, M. (2014). Response to phosphorus limitation varies among lake populations of the freshwater snail Potamopyrgus antipodarum. PLoS ONE, 9(1), 1– 5. https://doi.org/10.1371/journal.pone.0085845  

Kumar, S., Jones, M., Koutsovoulos, G., Clarke, M., & Blaxter, M. (2013). Blobology: Exploring raw genome data for contaminants, symbionts and parasites using taxon‐annotated GC‐coverage plots. Frontiers in Genetics, 4, 1– 12. https://doi.org/10.3389/fgene.2013.00237 

Laine, A. L. (2009). Role of coevolution in generating biological diversity: Spatially divergent selection trajectories. Journal of Experimental Botany, 60, 2957– 2970. https://doi.org/10.1093/jxb/erp168 

Lively, C. M. (1987). Evidence from a New Zealand snail for the maintenance of sex by parasitism. Nature, 328, 519– 521. https://doi.org/10.1038/328519a0 

Neiman, M., & Lively, C. M. (2004). Pleistocene glaciation is implicated in the phylogeographic structure of a New Zealand freshwater snail, Potamopyrgus antipodarum. Molecular Ecology, 13, 3085– 3098. https://doi.org/10.1111/j.1365-294X.2004.02292.x 

Neiman, M., Paczesniak, D., Soper, D. M., Baldwin, A. T., & Hehman, G. (2011). Wide variation in ploidy level and genome size in a New Zealand freshwater snail with coexisting sexual and asexual lineages. Evolution, 65, 3202– 3216. https://doi.org/10.1111/j.1558-5646.2011.01360.x 

Osnas, E. E., & Lively, C. M. (2005). Immune response to sympatric and allopatric parasites in a snail‐trematode interaction. Frontiers in Zoology, 2, 1– 7. https://doi.org/10.1186/1742-9994-2-8 

Ozerov, M. Y., Himberg, M., Aykanat, T., Sendek, D. S., Hägerstrand, H., Verliin, A., … Vasemäge, A. (2015). Generation of a neutral FST baseline for testing local adaptation on gill raker number within and between European whitefish ecotypes in the Baltic Sea Basin. Journal of Evolutionary Biology, 28, 1170– 1183. https://doi.org/10.1111/jeb.12645 

Paczesniak, D., Jokela, J., Larkin, K., & Neiman, M. (2013). Discordance between nuclear and mitochondrial genomes in sexual and asexual lineages of the freshwater snail Potamopyrgus antipodarum. Molecular Ecology, 22, 4695– 4710. https://doi.org/10.1111/mec.12422 

Paterson, S., Vogwill, T., Buckling, A., Benmayor, R., Spiers, A. J., Thomson, N. R., … Brockhurst, M. A. (2010). Antagonistic coevolution accelerates molecular evolution. Nature, 464, 275– 279. https://doi.org/10.1038/nature08798 

Smith, S. A., Wilson, N. G., Goetz, F. E., Feehery, C., Andrade, S. C. S., Rouse, G. W., … Dunn, C. W. (2011). Resolving the evolutionary relationships of molluscs with phylogenomic tools. Nature, 480, 364– 367. https://doi.org/10.1038/nature10526 

Tennessen, J. A., Théron, A., Marine, M., Yeh, J. Y., Rognon, A., & Blouin, M. S. (2015). Hyperdiverse gene cluster in snail host conveys resistance to human schistosome parasites. PLoS Genetics, 11, 1– 21. https://doi.org/10.1371/journal.pgen.1005067 

Trapnell, C., Hendrickson, D. G., Sauvageau, M., Goff, L., Rinn, J. L., & Pachter, L. (2013). Differential analysis of gene regulation at transcript resolution with RNA‐seq. Nature Biotechnology, 31, 46– 53. https://doi.org/10.1038/nbt.2450 

Trapnell, C., Roberts, A., Goff, L., Pertea, G., Kim, D., Kelley, D. R., … Patcher, L. (2012). Differential gene and transcript expression analysis of RNA‐Seq experiments with TopHat and Cufflinks. Nature Protocols, 7, 562– 578. https://doi.org/10.1038/nprot.2012.016 

Trapnell, C., Williams, B. A., Pertea, G., Mortazavi, A., Kwan, G., van Baren, M. J., … Pachter, L. (2010). Transcript assembly and quantification by RNA‐Seq reveals unannotated transcripts and isoform switching during cell differentiation. Nature Biotechnology, 28, 511– 515. https://doi.org/10.1038/nbt.1621 

Vergara, D., Lively, C. M., King, K. C., & Jokela, J. (2013). The geographic mosaic of sex and infection in lake populations of a New Zealand snail at multiple spatial scales. American Naturalist, 182, 484– 493. https://doi.org/10.1086/671996 

Wilton, P. R., Sloan, D. B., Logsdon, J. M. Jr., Doddapaneni, H., & Neiman, M. (2013). Characterization of transcriptomes from sexual and asexual lineages of a New Zealand snail (Potamopyrgus antipodarum). Molecular Ecology Resources, 13, 289– 294. https://doi.org/10.1111/1755-0998.12051 

Winterbourn, M. L. (1973). Larval trematode parasitising the New Zealand species of Potamopyrgus (Gastropoda: Hydrobiidae). Mauri Ora, 2, 17– 30. 

