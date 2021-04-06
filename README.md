# Introduction

[Bankers, et al 2017](https://onlinelibrary.wiley.com/doi/epdf/10.1111/mec.14146)

Bankers, L, Fields, P, McElroy, KE, Boore, JL, Logsdon, JM, Neiman, M. Genomic evidence for population‐specific responses to co‐evolving parasites in a New Zealand freshwater snail. 
Mol Ecol. 2017; 26: 3663– 3675. https://doi.org/10.1111/mec.14146

>Co‐evolving interactions between hosts and parasites create strong selection that can promote rapid, specific evolution. That said, we still only have a limited knowledge of how coevolution
 works in host-parasite relationships on a genomic level. Here, Bankers, et al, analyzes gene expression and sequence mutation to bridge that gap in knowledge between Potamopyrgus antipodarum
 and Microphallus sp., a sterilizing trematode parasite. They found systematic downregulation of many genes in infected P. antipodarum in relation to their uninfected counterparts, but the
 genes experiencing this change in expression differ depending on source location of each snail population, which is consistent with populaiton-level coevolution turning into population-specific
 host-parasite interactions.


![N|Solid](https://onlinelibrary.wiley.com/cms/asset/a8e764af-bab5-4fd6-b0c5-89c880344feb/mec14146-fig-0001-m.jpg)


*"Heatmaps representing significantly differentially expressed transcripts (higher FPKM = higher expression). Significance was assessed with a
 FDR of 5% and Benjamini‐Hochberg multiple test correction. (a) Inclusive analysis: 1,408 significantly differentially expressed transcripts in
 infected vs. uninfected snails. Transcripts above the black line demarcated with an astricks are downregulated in infected snails (1,057), and
 transcripts below this line are upregulated in infected snails (351). (b) Within‐lake analysis: dendrogram and heatmap representing the 6,228
 significantly differentially expressed transcripts across infection status and lakes. “Ax” = Alexandrina, “Se” = Selfe, “Kn” = Kaniere, red = infected,
 blue = uninfected. Snails clustered by lake of origin rather than infection status, indicating spatially structured gene expression patterns. Highlighted
 regions of heatmap contain examples of: expression differences between infected and uninfected snails within a lake (green), lake‐specific expression
 regardless of infection status (downregulation in Ax, blue) and across‐lake upregulation in infected snails (purple)"(Bankers 2017)*

This figure shows the relative expression levels of many genes across populations from differing origins.
 While panel (a) shows an all-inclusive analysis, panel
 (b) breaks the analysis down by source lake, highlighting the changes in host-parasite relationship and evolution trajectory. This figure shows 
 that there is a clear downregulation in the expression of certain genes, marked with an asterick, in uninfected snails.

# Materials and Methods

## Data

I was able to obtain the full transcriptome and the CuffDiff outputs from the author of the paper, which will greatly help my process. The 
transcriptome is the full transcriptome for Potamopyrgus antipodarum, and it can be found in this project's GitHub repository or on the Neiman Lab [website.] (http://bioweb.biology.uiowa.edu/neiman/Potamomics.php)
The CuffDiff output zip folders are available through my project [repository] (https://github.com/Intro-Sci-Comp-UIowa/biol-4386-course-project-cmhggns/tree/main/data) only, as it includes unpublished data.
The CuffDiff outputs are essentially estimates of the number of fragments of each transcript and gene in the transcriptome. This helps determine
the gene count of genes of interest, giving us the ability to track the expression of our target genes. When we compare the CuffDiff output to 
the reference genome, which is the genome of Potamopyrgus antipodarum found in Lake Alexandrina in New Zealand, we can look for signatures of selection
and determine what genes are being upregulated (or downregulated) in infected versus uninfected populations. This process is outlined below.


* Here's the shasum value for the transcriptome - 741a6a2e0e337034a5a3957b7fc2088d7e39e459  transcriptome *


## Methods

### Initiallizing the CummeRbund program
First, I downloaded R and cummeRbund. I uploaded the CuffLinks output files from Dr. Bankers into my R project, and I unzipped the files. From there,
I attempted to follow the same commands that worked in the previous project, without success. The code I attempted to execute is below.

```{r}
# Call cummeRbund and ask it to read the CuffLinks files.
>library(cummeRbund)
>cuff<-readCufflinks()
>cuff
# (This will show the cuffset, it will show nothing if it didn't work)
# When I performed this action, the command returned nothing

# To filter down to significantly differentially expressed genes:
>sig<-getSig(cuff, alpha=0.05, level='genes')
>sigGenes<-getGenes(cuff,sig)
>sigGenes

# To make the heatmap of differentially expressed genes:
>h<-csHeatmap(sigGenes,cluster='both')
>h
>png(filename = 'thin_heatmap.png', width = 400, height = 1000, units = 'px')
>csHeatmap(sigGenes,cluster='both')
>dev.off()
# Ethan has suggested using ComplexHeatmap or another program because R's standard heatmap() function is unintuitive.

# To make the dendrogram above the heatmap in 1B:
>den<-csDendro(genes(cuff))
>den
```

### Prior Data Acquisition
Thankfully, I already have access to the CuffDiff outputs. If I didn't, I could have used Cufflinks to run the transcriptome file in the CuffDiff
program. Cufflinks is commonly used for transcriptome assembly and differential expression analysis for RNA-seq data, and it is freely avialble
online, [here.] (http://cole-trapnell-lab.github.io/cufflinks/cuffdiff/) I already have the data from this, but if you don't, you could simply
follow these commands:

```{r}
cuffdiff [options]* <transcripts.gtf> \
<sample1_replicate1.sam[,…,sample1_replicateM.sam]> \
<sample2_replicate1.sam[,…,sample2_replicateM.sam]> … \
[sampleN.sam_replicate1.sam[,…,sample2_replicateM.sam]]
```

# Discussion

I am stuck at the cuff command, as noted above. I've ran the cuff command with several iterations, and I have yet to get it to work. Supposedly, 
