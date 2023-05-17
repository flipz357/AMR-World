# Overview of free AMR tools and resources

An overview over available tools for doing all kinds of tasks on AMR graphs. Requirements to be included

- free usage
- small dependencies
- no parsing or generation (should be listed separately)

## AMR tools

### Graph processing, reading, writing

- [penman](https://github.com/goodmami/penman),  [📜](https://www.aclweb.org/anthology/2020.acl-demos.35/): library for reading, writing and manipulating graphs
                                                  
### AMR metrics & AMR-to-AMR alignment

- [Smatch](https://github.com/snowblink14/smatch), [📜, 2013](https://aclanthology.org/P13-2131/): structural graph similarity, one-to-one node alignment
- [Smatch++](https://github.com/flipz357/smatchpp), [📜, 2023](https://aclanthology.org/2023.findings-eacl.118/): optimal/standardized Smatch and subgraph Smatch
- [WWLK](https://github.com/flipz357/weisfeiler-leman-amr-metrics), [📜,2021](https://aclanthology.org/2021.tacl-1.85/): Graded Weisfeiler Leman Kernel for AMR with glove embeddings, many-to-many alignment 

### AMR-to-text alignment

- [JAMR-aligner](https://github.com/jflanigan/jamr), [📜, 2014](https://jflanigan.github.io/flanigan+etal.acl2014.pdf), alignment as parsing step
- [GPLA-aligner](https://github.com/ChunchuanLv/AMR_AS_GRAPH_PREDICTION), [📜, 2018]((https://aclanthology.org/P18-1037/), alignment as parsing step
- [Leamr](https://github.com/ablodge/leamr), [📜, 2021](https://aclanthology.org/2021.acl-long.257/):  Statistical amr-text aligmemnt
- [WWLK-aligner](https://github.com/flipz357/weisfeiler-leman-amr-metrics), [📜, 2021](https://aclanthology.org/2021.tacl-1.85/): Wasserstein amr-text alignment  


