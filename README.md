# TSS-Captur: A TSS-characterization pipeline for transcribed but unclassified RNA-transcripts
Developed by Mathias Witte Paz

M.Sc. Bioinformatics

University of Tübingen

To enable the characterization of transcripts in an explorative manner, we have developed TSS-Captur. TSS-Captur characterizes transcripts starting on clear TSS signals obtained from TSSpredator (Herbig, 2015) that cannot be associated to any known gene. To characterize the function of the transcript, TSS-Captur integrates tools using different approaches. The following figure describes the different steps and tools run by TSS-Captur. 

![EplanationMethods](https://user-images.githubusercontent.com/29492782/119950451-2403d880-bf9b-11eb-9b3e-326408f47c53.png)

It combines the advantages of comparative genomics and _ab initio_ methods to account for many characteristics in the prediction. Furthermore, it uses the approach of transcriptional-signal based tools to combine TSS signals with a possible terminator. Moreover, it enables the user to explore the thermodynamic characteristics of possible identified ncRNA transcripts and visualize the secondary structure. Lastly, it facilitates the analysis of motifs within the promoter regions before each TSS signal to identify possible binding sites or other regulatory elements. All these results are combined within an interactive interface. This interface does not only provide an overview of the predicted results, but offers the possibility of getting the detailed information for each transcript and hence being able to reconstruct the predictions done by TSS-Captur.

------
How to run: 
``` bash
./nextflow run tss_captur.nf --inputTable [PATH_TO_MASTER_TABLE] --inputGenomes [PATH_TO_GENOMES_DIR] --inputGFFs [PATH_TO_GFF_DIR] --outputDir [PATH_TO_OUTPUT] --blastdb [PATH_TO_NT_DB]  -with-docker mwittep/tsscaptur 

```
