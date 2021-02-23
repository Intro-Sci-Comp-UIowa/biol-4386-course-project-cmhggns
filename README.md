*Chelsea Higgins Homework 1* 

  

# Populations specific responses of P. antipodarum to co-evolving parasites, as shown by genomic evidence 

  

### [Bankers, et al 2017](https://onlinelibrary.wiley.com/doi/epdf/10.1111/mec.14146) 

Bankers, L, Fields, P, McElroy, KE, Boore, JL, Logsdon, JM, Neiman, M. Genomic evidence for population‐specific responses to co‐evolving parasites in a New Zealand freshwater snail. Mol Ecol. 2017; 26: 3663– 3675. https://doi.org/10.1111/mec.14146 

  

## Introduction 

  

>Co‐evolving interactions between hosts and parasites create strong selection that can promote rapid, specific evolution.That said, we still only have a limited knowledge of how coevolution works in host-parasite relationships on a genomic level. Here, Bankers, et al, analyzes gene expression and sequence mutation to bridge that gap in knowledge between Potamopyrgus antipodarum and Microphallus sp., a sterilizing trematode parasite. They found systematic downregulation of many genes in infected P. antipodarum in relation to their uninfected counterparts, but the genes experiencing this change in expression differ depending on source location of each snail population, which is consistent with populaiton-level coevolution turning into population-specific host-parasite interactions. 

  

## Figure to Reproduce 

  

![N|Solid](https://onlinelibrary.wiley.com/cms/asset/a8e764af-bab5-4fd6-b0c5-89c880344feb/mec14146-fig-0001-m.jpg) 

*This figure shows the relative expression levels of many genes across populations from differing origins, with a higher FPKM signaling higher expression. There is a clear downregulation in expression of certain genes, marked with an astrick, in uninfected snails. Panel (a) shows an all-inclusive analysis with 1,408 significantly differentially expressed transcripts, depending on infection status. 1,057 transcripts were downregulated in infected snails, shown above the black line with an astericks, whereas the data below the line shows the 351 transcripts upregulated in infected snails. Panel (b) breaks the analysis down by source lake, representing 6,228 significantly diferentially expressed transcripts, highlighting the changes in host-parasite relationship and evolution trajectory. Ax = Alexandrina, Se = Selfe, Kn = Kaniere, red = infected, and blue = uninfected. Snails are grouped by lake of origin, showing gene expression patterns that may be structured spatially. The green box indicates expression diferences by infection status within a lake. The blue box shows lake-specific expression without considering infection status, and the purple box displays the upregulation of transcripts in infected snails across lakes.* 

  

## Materials and Methods 

  

- This figure was created by using RNA-sequencing and de novo reference transcriptome editing and annotation. The authors then used specialized programs CUFFLINKS, TOPHAT, and CUFFMERGE together to analyze the data in CUFFDIF, another specialized program. After analysis, the authors used cummeRbund to visualize the data as a heat map. 

- Fortunately, I already have this data, but I have a better assembly. Laura, the first author on this paper, along with most of the other authors, are all alumni of my research group, and I keep up with them regulary, regarding my own research. I have the original sequencing data and an improved assembly in my lab database. 

- In order to reproduce this figure, I will follow the same steps Laura did. I will take my newer assembly and upload it into CUFFDIF. I will create a table that tracks transcripts with a significant difference between infected and uninfected snails, like Table S2 in Bankers, 2017, using the same variables she did (two fold changes in gene expression and at least 4 fragments per kilobase per million reads mapped [FPKM]). Finally, I will use cummeRbund to visualize that table as a heat map.  

  

If I run into any trouble throughout this process, I am meeting with Laura regularly for my thesis project, so I can get a quick response to any questions I may have. Additionally, Laura presented every step of her process in tables, found in the supplementary materials to this paper.

