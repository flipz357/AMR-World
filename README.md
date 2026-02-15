# AMR World 🌎: *Open* AMR tools and resources 

An overview of available tools and resources for AMR graphs. Requirements to be included are:

- Publicly available (main requirement)
- If it's a tool: easy to use (ideally)

Please file an issue or make a pull request if you want to make a suggestion for inclusion. There should be a link to a github-repository and (if available) a link to a related publication (📜). Note that work/papers on single parsers or generators should be listed separately, except if they are easy to use off-the-shelf.

## Table of Contents

- [AMR Data](#amr-data)
  - [Standard English Sembanks](#standard-english-sembanks)
  - [Other Languages](#Other-Languages)
  - [Pair-wise annotations](#Pair-wise-annotations)
  - [Miscelanea](#Miscelanea)
- [AMR Tools](#amr-tools)
  - [Parsing and Generation](#Parsing-and-Generation)
  - [Annotation and Visualization](#Annotation-and-Visualization)
  - [Graph reading, writing, standardization](#Graph-reading-writing-standardization)
  - [Metrics and Evaluation](#Metrics-and-Evaluation)
  - [Graph-to-text alignment](#Graph-to-text-alignment)

Elements in each categorty are sorted alphabetically. 

## AMR Data

### Standard English Sembanks

Please find information about the "traditional/long-standing" English public manual AMR annotations in [this sub-directory](https://github.com/flipz357/AMR-World/tree/main/data/reference_amrs). 

### Other Languages

Non-English Sembanks contain Non-English texts and their AMR graphs.

- [Brazilian AMR](https://github.com/rafaelanchieta/amr-br), [📜](https://aclanthology.org/L18-1157/): 1561 Brazilian AMRs for Little Prince. Manually created.
- [Chinese AMR](http://www.cs.brandeis.edu/~clp/camr/camr.html) [📜](https://aclanthology.org/W16-1702/): 1562 Chinese AMRs for Little Prince. Manually crafted. Double annotated.
- [German AMR](https://github.com/chriott/deamr), [📜](https://aclanthology.org/2024.lrec-main.26/): 400 German AMRs. Manually created.
- [Spanish AMR](https://github.com/shirawein/Spanish-Abstract-Meaning-Representation),  [📜](https://nejlt.ep.liu.se/article/view/4462/3648): 486 AMRs (source sentences available through Linguistic Data Consortium). Manually created.
- [Korean AMR](https://github.com/choe-hyonsu-gabrielle/korean-amr-corpus), [📜](https://www.aclweb.org/anthology/2020.dmr-1.3/): 1,253 sentences. Manually created.
- [Turkish AMR](https://github.com/amr-turkish/turkish-amr-corpus), [📜](https://aclanthology.org/P19-2006/): 700 gold sentences.

English Sembanks that relate to other languages.

- [MASSIVE AMR](https://github.com/amazon-science/MASSIVE-AMR), [📜](https://aclanthology.org/2024.starsem-1.1/): A dataset with more than 84,000 text-to-graph Abstract Meaning Representation (AMR) annotations for 1,685 information-seeking utterances mapped to 50+ typologically diverse languages. Manually created.

### Pair-wise annotations

Pairs of AMRs with annotation, e.g., entailment, or similarity.

- [BAMBOO benchmark](https://github.com/flipz357/bamboo-amr-benchmark), [📜](https://aclanthology.org/2021.tacl-1.85/): Several thousand similarity-annotated pairs of silver AMRs for testing and evaluating AMR metrics.
- [Chinese AMR Double Annotation](http://www.cs.brandeis.edu/~clp/camr/camr.html) [📜](https://aclanthology.org/W16-1702/): 1562 Chinese AMRs for Little Prince. Manually crafted. Double annotated.
- [NLI AMR](https://github.com/flipz357/amr4nli), [📜](https://arxiv.org/abs/2306.00936): >1 mio Silver AMR pairs of five NLI data sets.
- [Spanish-English](https://github.com/shirawein/spanish-english-amr-corpus), [📜](https://aclanthology.org/2021.law-1.6/): 50 pairs of parallel AMRs with annotated divergence type. Manually crafted.
- [ParsEval](https://github.com/Heidelberg-NLP/AMRParseEval), [📜](https://aclanthology.org/2022.eval4nlp-1.4/): 800 Parsed AMRs with human quality annoations (domain: little Prince, AMR3).

### Miscelanea

- [AMR Bibliography](https://github.com/nert-nlp/AMR-Bibliography), [📜](https://nert-nlp.github.io/AMR-Bibliography/): Continuously updated collection of publications related to AMR.
- [AMR dictionaries and lexica](https://github.com/flipz357/AMR-World/tree/main/data/dictionaries)
- [AMR Guidelines](https://github.com/amrisi/amr-guidelines/blob/master/amr.md), [📜](https://aclanthology.org/W13-2322/): AMR examples, and how to create AMRs.
- [GrAPES](https://github.com/jgroschwitz/GrAPES), [📜](https://arxiv.org/abs/2312.03480): AMR parser challenge.
- [UMR](https://umr4nlp.github.io/web/): Uniform Meaning Representation is a successor to AMR that aims to be more flexible across languages and to cover more semantic phenomena.

## AMR Tools

If not mentioned otherwise, tools are all in Python.

### Parsing and Generation

These are tools for generating AMRs from text (parsing), or generating text from AMR (generation). 

- [amrlib](https://github.com/bjascob/amrlib): Many pre-trained (English) models for parsing and generation.

### Annotation and Visualization

(Usually) GUI-based tools for creating, saving, and showing AMRs

- [metamorphosed](https://github.com/Orange-OpenSource/metamorphosed), [📜](https://aclanthology.org/2023.isa-1.4/): graphical editor to edit Abstract Meaning Representations graphs

### Graph reading, writing, standardization

These are tools for reading, writing and handling AMR graphs.

- [amr-utils](https://github.com/ablodge/amr-utils): read, write, visualize graphs
- [penman](https://github.com/goodmami/penman),  [📜](https://www.aclweb.org/anthology/2020.acl-demos.35/): read, write, modify graphs
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): read, write, modify graphs, standardize graphs

### Metrics and Evaluation

#### Structure matching 

The following are graph metrics that compare graphs structurally (i.e., they don't use embeddings etc.). 

- [Ancast](https://github.com/sxndqc/ancast), [📜](https://aclanthology.org/2024.lrec-main.94/): Approximates Smatch, more efficient than Smatch.
- [Sema](https://github.com/rafaelanchieta/sema), [📜](https://arxiv.org/abs/1905.12069): triple match heuristic, fast.
- [SemBleu](https://github.com/freesunshine0316/sembleu), [📜](https://aclanthology.org/P19-1446/): path extraction heuristic, fast.
- [Smatch](https://github.com/snowblink14/smatch), [📜](https://aclanthology.org/P13-2131/): triple match, heuristic solver.
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): triple match, optimal solver, standardized scoring. Fine-grained scoring.

#### Structure and content matching

These are "advanced" metrics that use embeddings or other features, for finer graph meaning similarity (e.g., structures like `kitten` vs. `cat` vs. possibly `cat :mod young`, etc.). 

- [AMRSim](https://github.com/zzshou/AMRSim), [📜](https://aclanthology.org/2023.acl-long.892/): Self supervised learning of graph matching witn neural network
- [CALAMR](https://github.com/uic-nlp-lab/calamr), [📜](https://aclanthology.org/2024.lrec-main.236/): Flow-based alignment of graph components
- [Rematch](https://github.com/osome-iu/Rematch-RARE), [📜](https://arxiv.org/abs/2404.02126): Efficient graph feature matching with node label generalization
- [S2match](https://github.com/Heidelberg-NLP/amr-metric-suite), [📜](https://aclanthology.org/2020.tacl-1.34/): Smatch with word embeddings
- [SXmatch](https://github.com/shirawein/Crossling-AMR-Eval), [📜](https://aclanthology.org/2022.coling-1.336/): Smatch with cross-lingual embeddings
- [WWLK](https://github.com/flipz357/weisfeiler-leman-amr-metrics), [📜](https://aclanthology.org/2021.tacl-1.85/): Contextualized matching with Wasserstein distance Weisfeiler Leman Algorithm


### Graph-to-text alignment

These are methods for finding out which parts of two AMRs relate to which parts of a sentence.

- [GPLA-aligner](https://github.com/ChunchuanLv/AMR_AS_GRAPH_PREDICTION), [📜](https://aclanthology.org/P18-1037/), alignment as parsing step
- [JAMR-aligner](https://github.com/jflanigan/jamr), [📜](https://aclanthology.org/P14-1134/), alignment as parsing step
- [Leamr](https://github.com/ablodge/leamr), [📜](https://aclanthology.org/2021.acl-long.257/):  Learned statistical amr-text aligmemnt
- [WWLK-aligner](https://github.com/flipz357/Simple-AMR-Aligner), [📜](https://aclanthology.org/2021.tacl-1.85/): Wasserstein amr-text alignment

