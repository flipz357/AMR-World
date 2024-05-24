# AMR World 🌎: *free* AMR tools and resources 🎊

An overview of available tools and resources for AMR graphs. Requirements to be included are:

- free usage (main requirement)
- easy to use (ideally)

Please file an issue or make a pull request if you want to make a suggestion for inclusion. There should be a link to a github-repository and (if available) a link to a related publication (📜). Note that work/papers on single parsers or generators should be listed separately, except if they are easy to use off-the-shelf.

Elements are sorted alphabetically.

## AMR tools

If not mentioned otherwise, tools are all in Python.

### Parsing & generation

These are tools for generating AMRs from text (parsing), or generating text from AMR (generation).

- [amrlib](https://github.com/bjascob/amrlib): Many pre-trained (English) models for parsing and generation.

### Graph reading, writing

These are tools for reading, writing and handling AMR graphs.

- [amr-utils](https://github.com/ablodge/amr-utils): read, write, modify graphs
- [penman](https://github.com/goodmami/penman),  [📜](https://www.aclweb.org/anthology/2020.acl-demos.35/): read, write, modify graphs
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): read, write, modify graphs

### Graph processing/transformation

-  [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): extract subgraphs, standardize graphs

### Metrics & Graph alignment

#### Structure matching 

The following are graph metrics that compare meaning graphs structurally (i.e., they don't use embeddings etc.). 

- [Ancast](https://github.com/sxndqc/ancast), [📜](https://aclanthology.org/2024.lrec-main.94/): Approximates Smatch, more efficient than Smatch
- [Sema](https://github.com/rafaelanchieta/sema), [📜](https://arxiv.org/abs/1905.12069): triple match heuristic, fast
- [SemBleu](https://github.com/freesunshine0316/sembleu), [📜](https://aclanthology.org/P19-1446/): path extraction heuristic, fast
- [Smatch](https://github.com/snowblink14/smatch), [📜](https://aclanthology.org/P13-2131/): triple match, heuristic solver
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): triple match, optimal solver, standardized scoring. 

#### Structure and content matching

These are metrics that use embeddings or other features, for finer graph meaning similarity (e.g., structures like `kitten` vs. `cat` vs. possibly `cat :mod young`, etc.). 

- [AMRSim](https://github.com/zzshou/AMRSim), [📜](https://aclanthology.org/2023.acl-long.892/): Self supervised learning of graph matching witn neural network
- [CALAMR](https://github.com/uic-nlp-lab/calamr), [📜](https://aclanthology.org/2024.lrec-main.236/): Flow-based alignment of graph components
- [Rematch](https://github.com/osome-iu/Rematch-RARE), [📜](https://arxiv.org/abs/2404.02126): Efficient graph feature matching with node label generalization
- [S2match](https://github.com/Heidelberg-NLP/amr-metric-suite), [📜](https://aclanthology.org/2020.tacl-1.34/): Smatch with word embeddings
- [SXmatch](https://github.com/shirawein/Crossling-AMR-Eval), [📜](https://aclanthology.org/2022.coling-1.336/): Smatch with cross-lingual embeddings
- [WWLK](https://github.com/flipz357/weisfeiler-leman-amr-metrics), [📜](https://aclanthology.org/2021.tacl-1.85/): Contextualized matching with Wasserstein distance Weisfeiler Leman Algorithm

#### Graph alignment

These are methods for finding out which parts of two AMRs relate to eath other. Most are based on a side-product from computing a metric.

- Align nodes: Smatch, S2match, XSmatch
- Align broader structures: WWLK

### Graph-to-text alignment

These are methods for finding out which parts of two AMRs relate to which parts of a sentence.

- [GPLA-aligner](https://github.com/ChunchuanLv/AMR_AS_GRAPH_PREDICTION), [📜](https://aclanthology.org/P18-1037/), alignment as parsing step
- [JAMR-aligner](https://github.com/jflanigan/jamr), [📜](https://aclanthology.org/P14-1134/), alignment as parsing step
- [Leamr](https://github.com/ablodge/leamr), [📜](https://aclanthology.org/2021.acl-long.257/):  Learned statistical amr-text aligmemnt
- [WWLK-aligner](https://github.com/flipz357/Simple-AMR-Aligner), [📜](https://aclanthology.org/2021.tacl-1.85/): Wasserstein amr-text alignment 

## AMR resources

### Sembanks: English

English Sembanks contain English texts and their AMR graphs.

- [Bio AMR](https://amr.isi.edu/download/2018-01-25/amr-release-bio-v3.0.txt): 6952 AMR annotated sentences from bio-medical domain
- [Little Prince AMR](https://amr.isi.edu/download/amr-bank-struct-v1.6.txt): 1562 AMR annotated sentences of the novel "little Prince"

The largest English AMR sembanks, as well as translations of many of their sentences into other languages, are unfortunately not open datasets (they are licensed through the Linguistic Data Consortium).

### Sembanks: Other languages

Non-English Sembanks contain Non-English texts and their AMR graphs.

- [Spanish AMR corpus](https://github.com/shirawein/Spanish-Abstract-Meaning-Representation),  [📜](https://nejlt.ep.liu.se/article/view/4462/3648): 486 gold AMRs (source sentences available through Linguistic Data Consortium)

### Pair-wise annotations

Pairs of AMRs with annotation, e.g., entailment, or similarity.

- [BAMBOO benchmark](https://github.com/flipz357/bamboo-amr-benchmark), [📜](https://aclanthology.org/2021.tacl-1.85/): testing and evaluating AMR metrics
- [NLI AMR](https://github.com/flipz357/amr4nli), [📜](https://arxiv.org/abs/2306.00936): >1 mio Silver AMR pairs of five NLI data sets
- [Spanish-English](https://github.com/shirawein/spanish-english-amr-corpus), [📜](https://aclanthology.org/2021.law-1.6/): 50 pairs of parallel AMRs with annotated divergence type
- [ParsEval](https://github.com/Heidelberg-NLP/AMRParseEval), [📜](https://aclanthology.org/2022.eval4nlp-1.4/): 800 Parsed AMRs with human quality annoations (domain: little Prince, AMR3)
- [Textual Similarity](https://github.com/flipz357/bamboo-amr-benchmark), [📜](https://aclanthology.org/2021.tacl-1.85/): Silver AMRs of text similarity benchmarks (e.g., STS) that are annoated with human textual similarity ratings

### Other resources

- [AMR Bibliography](https://github.com/nert-nlp/AMR-Bibliography), [📜](https://nert-nlp.github.io/AMR-Bibliography/): Up-to-date and very large collection of publications on AMR.
- [AMR Guidelines](https://github.com/amrisi/amr-guidelines/blob/master/amr.md), [📜](https://aclanthology.org/W13-2322/): The backbone of everything. AMR examples, and how to create AMRs.
- [AMR Dictionary](https://www.isi.edu/~ulf/amr/lib/amr-dict.html): Fine-grained specification of AMR roles, special frames, entity types, etc.
- [GrAPES](https://github.com/jgroschwitz/GrAPES), [📜](https://arxiv.org/abs/2312.03480): AMR parser challenge
- [UMR](https://umr4nlp.github.io/web/): Uniform Meaning Representation is a successor to AMR that aims to be more flexible across languages and to cover more semantic phenomena.
