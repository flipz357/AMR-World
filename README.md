# Overview AMR tools and resources

An overview over available tools for doing all kinds of tasks on AMR graphs. Requirements to be included

- free usage
- small dependencies
- no parsing or generation (should be listed separately)

## AMR tools

### Graph processing, reading, writing

- [penman](https://github.com/goodmami/penman),  [📜](https://www.aclweb.org/anthology/2020.acl-demos.35/): library for reading, writing and manipulating graphs
                                                  
### AMR metrics & AMR-to-AMR alignment

- [Smatch](https://github.com/snowblink14/smatch), [📜](https://aclanthology.org/P13-2131/): structural graph similarity, one-to-one node alignment with hill-climber
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): optimal/standardized Smatch and subgraph Smatch
- [WWLK](https://github.com/flipz357/weisfeiler-leman-amr-metrics), [📜](https://aclanthology.org/2021.tacl-1.85/): Graded Weisfeiler Leman Kernel for AMR with glove embeddings, many-to-many alignment 

### AMR-to-text alignment

- [JAMR-aligner](https://github.com/jflanigan/jamr), [📜](https://jflanigan.github.io/flanigan+etal.acl2014.pdf), alignment as parsing step
- [GPLA-aligner](https://github.com/ChunchuanLv/AMR_AS_GRAPH_PREDICTION), [📜](https://aclanthology.org/P18-1037/), alignment as parsing step
- [Leamr](https://github.com/ablodge/leamr), [📜](https://aclanthology.org/2021.acl-long.257/):  Statistical amr-text aligmemnt
- [WWLK-aligner](https://github.com/flipz357/Simple-AMR-Aligner), [📜](https://aclanthology.org/2021.tacl-1.85/): Wasserstein amr-text alignment 

## AMR resources

### AMR sembanks: English

- [Little Prince AMR](https://amr.isi.edu/download/amr-bank-struct-v1.6.txt): 1562 AMR annotated sentences of the novel "little Prince"
- [Bio AMR](https://amr.isi.edu/download/2018-01-25/amr-release-bio-v3.0.txt): 6952 AMR annotated sentences from bio-medical domain

### AMR sembanks: Other languages

- [Spanish AMR corpus](https://github.com/shirawein/Spanish-Abstract-Meaning-Representation),  [📜](https://nejlt.ep.liu.se/article/view/4462/3648): 486 gold-annotated sentences spanning multiple genre

### Pair-wise annotations

- [Spanish-English](https://github.com/shirawein/spanish-english-amr-corpus), [📜](https://aclanthology.org/2021.law-1.6/): 50 pairs of parallel AMRs with annotated divergence type
- [Textual Similarity](https://github.com/flipz357/bamboo-amr-benchmark), [📜](https://aclanthology.org/2021.tacl-1.85/): Silver AMRs of text similarity benchmarks (e.g., STS) that are annoated with human textual similarity ratings
- [AMR ParsEval](https://github.com/Heidelberg-NLP/AMRParseEval), [📜](https://aclanthology.org/2022.eval4nlp-1.4/): 800 Parsed AMRs with human quality annoations (domain: little Prince, AMR3)


