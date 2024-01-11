# Overview of free AMR tools and resources

An overview of available tools for doing all kinds of tasks on AMR graphs. Requirements to be included are:

- free usage
- small dependencies (ideally)
- no parsing or generation (should be listed separately)

Please file an issue or make a pull request if you want to make a suggestion for inclusion. 

Elements are sorted alphabetically.

## AMR tools

### Graph processing, reading, writing

- [amr-utils](https://github.com/ablodge/amr-utils): read, write, modify graphs
- [penman](https://github.com/goodmami/penman),  [📜](https://www.aclweb.org/anthology/2020.acl-demos.35/): read, write, modify graphs
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): read, write, modify graphs, standardization
                                                  
### AMR metrics & AMR-to-AMR alignment

#### Structural matching

- [Sema](https://github.com/rafaelanchieta/sema), [📜](https://arxiv.org/abs/1905.12069): heuristic, fast
- [SemBleu](https://aclanthology.org/P19-1446/), [📜](https://github.com/freesunshine0316/sembleu): heuristic, fast
- [Smaragd](https://github.com/PhMeier/Smaragd/), [📜](https://arxiv.org/abs/2203.13226): heuristic (learned Smatch), fast
- [Smatch](https://github.com/snowblink14/smatch), [📜](https://aclanthology.org/P13-2131/): triple match, heuristic solver
- [Smatch++](https://github.com/flipz357/smatchpp), [📜](https://aclanthology.org/2023.findings-eacl.118/): triple match, optimal solver

#### Structure and content matching

- [S2match](https://github.com/Heidelberg-NLP/amr-metric-suite), [📜](https://aclanthology.org/2020.tacl-1.34/): Node labels matched via word embeddings
- [SXmatch](https://github.com/shirawein/Crossling-AMR-Eval), [📜](https://aclanthology.org/2022.coling-1.336/): Node labels matched with cross-lingual embeddings
- [WWLK](https://github.com/flipz357/weisfeiler-leman-amr-metrics), [📜](https://aclanthology.org/2021.tacl-1.85/): Contextualized matching, broader matches

#### AMR-to-AMR alignment

- Align nodes: Smatch, S2match, XSmatch
- Align structures: WWLK

### AMR-to-text alignment

- [GPLA-aligner](https://github.com/ChunchuanLv/AMR_AS_GRAPH_PREDICTION), [📜](https://aclanthology.org/P18-1037/), alignment as parsing step
- [JAMR-aligner](https://github.com/jflanigan/jamr), [📜](https://jflanigan.github.io/flanigan+etal.acl2014.pdf), alignment as parsing step
- [Leamr](https://github.com/ablodge/leamr), [📜](https://aclanthology.org/2021.acl-long.257/):  Learned statistical amr-text aligmemnt
- [WWLK-aligner](https://github.com/flipz357/Simple-AMR-Aligner), [📜](https://aclanthology.org/2021.tacl-1.85/): Wasserstein amr-text alignment 

## AMR resources

### AMR sembanks: English

- [Bio AMR](https://amr.isi.edu/download/2018-01-25/amr-release-bio-v3.0.txt): 6952 AMR annotated sentences from bio-medical domain
- [Little Prince AMR](https://amr.isi.edu/download/amr-bank-struct-v1.6.txt): 1562 AMR annotated sentences of the novel "little Prince"

### AMR sembanks: Other languages

- [Spanish AMR corpus](https://github.com/shirawein/Spanish-Abstract-Meaning-Representation),  [📜](https://nejlt.ep.liu.se/article/view/4462/3648): 486 gold-annotated sentences spanning multiple genre

### Pair-wise annotations

- [NLI AMR](https://github.com/flipz357/amr4nli), [📜](https://arxiv.org/abs/2306.00936): >1 mio Silver AMR pairs of five NLI data sets
- [Spanish-English](https://github.com/shirawein/spanish-english-amr-corpus), [📜](https://aclanthology.org/2021.law-1.6/): 50 pairs of parallel AMRs with annotated divergence type
- [ParsEval](https://github.com/Heidelberg-NLP/AMRParseEval), [📜](https://aclanthology.org/2022.eval4nlp-1.4/): 800 Parsed AMRs with human quality annoations (domain: little Prince, AMR3)
- [Textual Similarity](https://github.com/flipz357/bamboo-amr-benchmark), [📜](https://aclanthology.org/2021.tacl-1.85/): Silver AMRs of text similarity benchmarks (e.g., STS) that are annoated with human textual similarity ratings




