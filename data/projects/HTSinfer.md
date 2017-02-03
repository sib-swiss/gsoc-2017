##### Rationale

Since 2000 when the first human genome [1] was sequenced and assembled, the number of publicly available High Throughput Sequencing (HTS) data sets
has grown exponentially. A variety of new sequencing methodologies were developed (e.g. from 454 Life Sciences, [Illumina](https://www.illumina.com/), 
[Pacific Biosciences](http://www.pacb.com/)), which enabled the acquisition of many types of data, e.g. from genome or transcriptome sequencing, ribosome
footprinting, transcription factor crosslinking and immunoprecipitation etc. To host these data sets, databases such as the sequence read archive
([SRA](https://www.ncbi.nlm.nih.gov/sra)) were developed. This (and other) large repositories are a treasure trove of information that awaits to be mined
with ever new research questions in mind. Unfortunately, extracting and processing such data sets in new studies is not always seamless, because the
standards for annotating the samples are still in flux. Thus, meta-data that may be relevant for a new study are not readily available in the original
annotation of the samples. Nevertheless, it is frequently the case that this information can be inferred from the sequencing data. The aim of this project
is to develop a set of tools for automatic extraction of experimental parameters from publicly available sequencing samples.

##### Approach

The student should develop a package that accepts HTS datasets and is able to automatically identify characteristics of the experiment such as 
- The organism from which the samples were derived
- Type of captured molecule (RNA, DNA) 
- How the samples were sequenced (single/paired end)
- The orientation of the reads
- Adaptor sequences that were used in the experiment

##### Challenges

The two main challenges are to grasp the various techniques that were used in the experiments and their possible artifacts, and to develop highly performant
methods that allow the timely processing of thousands of sequencing data sets.

##### Requirements

The ideal student has:
- Interest in bioinformatics
- Strong programming skills: python, C or similar
- Experience with parallel programming
- Basic experience with Git

##### References

[1] Lander ES, et al. Initial sequencing and analysis of the human genome. Nature. 2001 Feb15;409(6822):860-921.
