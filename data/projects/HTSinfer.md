##### Rationale

Thanks to the availability of _next generation sequencing_ - or High Throughput Sequencing (HTS) - techniques since the mid 2000's, the number of publicly available sequencing data sets has tremendously increased since the first human genome was published in 2001 [1]. Now, modern sequencing methodologies (e.g. by [Illumina](https://www.illumina.com/), [Pacific Biosciences](http://www.pacb.com/) and [Oxford Nanopore Technologies](https://nanoporetech.com/)) enable the massive acquisition of many types of biological data, e.g. from genome or transcriptome sequencing, ribosome footprinting, transcription factor or RNA-binding protein crosslinking and immunoprecipitation etc. To host these data sets, databases such as the Sequence Read Archive ([SRA](https://www.ncbi.nlm.nih.gov/sra)) were built. These repositories are treasure troves of information that await to be mined with ever new research questions in mind. Unfortunately, extracting and processing such data sets in new studies is not always seamless, because the standards for annotating the samples are still in flux. Thus, metadata that may be relevant to address a new research question are not readily available in the original annotation of the samples. However, it is frequently the case that this information can be inferred from the sequencing data itself. The aim of this project is to develop a toolbox for the automatic extraction of experimental parameters from publicly available sequencing samples.

##### Approach

The student should develop a software package that accepts HTS data sets and is able to automatically infer characteristics of the experiment such as

- the organism from which the samples were derived
- the type of the captured molecule (RNA, DNA) 
- how the samples were sequenced (single/paired end, read orientation)
- the _read architecture_, i.e. the layout of biologically relevant sequence fragments, adapters, linkers and barcodes
- the type of the experiment (RNA-Seq, genomic sequencing etc.)

![HTSinfer scheme](data/projects/images/HTSinfer_scheme.png)

##### Challenges

The two main challenges are to grasp the various techniques that were used in the experiments and their possible artifacts, and to develop highly performant methods that allow the timely processing of thousands of sequencing data sets.

##### Requirements

The ideal student has:

- Interest in bioinformatics
- Strong programming skills: C, Python or similar
- Strong background in mathematics/statistics and/or experience with machine learning techniques
- Experience with parallel computing
- Basic experience with Git

##### References

[1] Lander ES, et al. Initial sequencing and analysis of the human genome. Nature. 2001 Feb15;409(6822):860-921.
