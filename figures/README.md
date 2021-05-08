# Welcome to My Figures

### In this file, you will find the original figure, the figure I ended with, and an intermediate figure.
- To find out more about how this figure was reproduced, see the **methods** section.
- To learn about the differences between figures, see the **results** section.
- To read about what these figures even mean, read the **discussion** section.

-------------------

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

 
