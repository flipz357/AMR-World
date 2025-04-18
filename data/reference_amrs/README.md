# List of Human Reference AMR annotations

## Public data

### The Little Prince Corpus   version 3.0 · 1,562 sentences

This corpus is an annotation of the novel The Little Prince by Antoine de Saint-Exupéry, published in 1943. 

- [**The Little Prince corpus 3.0**](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-struct-v3.0.txt)

#### The Little Prince Corpus   version 1.6 · 1,562 sentences

- [**The Little Prince corpus 1.6**](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-struct-v1.6.txt), including meta data and Chinese translations.   Standard split: [145 dev AMRs](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-struct-v1.6-dev.txt), [1274 training AMRs](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-struct-v1.6-training.txt), [143 test AMRs](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-struct-v1.6-test.txt). 
- The Little Prince corpus in [simplified format](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-v1.6.txt), without meta data. 
- The Little Prince corpus in [xml format](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-bank-v1.6.xml), including meta data. 

### Bio AMR Corpus   version 3.0 · 6,952 sentences

This corpus includes annotations of cancer-related PubMed articles, covering 3 full papers ([PMID:24651010](http://www.ncbi.nlm.nih.gov/pubmed/24651010), [PMID:11777939](http://www.ncbi.nlm.nih.gov/pubmed/11777939), [PMID:15630473](http://www.ncbi.nlm.nih.gov/pubmed/15630473)) as well as the result sections of 46 additional PubMed papers. The corpus also includes about 1000 sentences each from the BEL BioCreative training corpus and the Chicago Corpus.

- [**The Bio AMR corpus**](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-release-bio-v3.0.txt)

#### Bio AMR Corpus   version 0.8 · 6,452 sentences

- Bio AMR corpus 0.8: [dev (500 snt.)](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-release-dev-bio.txt), [training (5,452 snt.)](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-release-training-bio.txt), [test (500 snt.)](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/amr-release-test-bio.txt)
- Aautomatically generated alignments for Bio AMR corpus 0.8: [dev (500 snt.)](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/alignment-release-dev-bio.txt), [training (5,452 snt.)](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/alignment-release-training-bio.txt), [test (500 snt.)](https://github.com/flipz357/AMR-World/blob/main/data/reference_amrs/alignment-release-test-bio.txt).


## Closed-source

- [LDC general release AMR 3.0](https://catalog.ldc.upenn.edu/LDC2020T02) on January 15, 2020, with 59,255 sentences. Includes multi-sentence annotations for part of the AMR corpus.
- [LDC general release AMR 2.0](https://catalog.ldc.upenn.edu/LDC2017T10) on June 15, 2017, with 39,260 sentences. 
- [SemEval Task 9](http://alt.qcri.org/semeval2017/task9) is AMR parsing and generation. Organized by Jonathan May. 

### Data that is not available (anymore)

- [LDC2013E117](https://catalog.ldc.upenn.edu/LDC2013E117): DEFT Phase 1 AMR Annotation R3 (October 24, 2013). 10,854 sentences with 13,050 AMRs (corpus includes multiple annotations for some sentences) · Release limited to DEFT participants.

## Sources

### Annotators of AMRs

The AMR Bank is manually constructed by human annotators at:

- [The Linguistic Data Consortium (LDC)](http://www.ldc.upenn.edu/)
- [SDL](http://www.sdl.com/)
- The University of Colorado's [Center for Computational Language and Education Research (CLEAR)](http://clear.colorado.edu/start)
- The University of Southern California's [Information Sciences Institute (ISI)](http://nlg.isi.edu/) and [Computational Linguistics at USC](http://cl.usc.edu/). 

### Data hosting

What is hosted on this page is taken from [the AMR-ISI webpage](https://amr.isi.edu/) that (currently) is unreachable. The data in this directory has been "rescued" via [Wayback Machine Link](https://web.archive.org/web/20231207171323/https://amr.isi.edu/).

### Acknowledgements

We repeat the acknowledgements from [the AMR-ISI webpage](https://amr.isi.edu/) that (currently) is unreachable: 

*Thanks to NSF (IIS-0908532) for funding the initial design of AMR, and to DARPA MRP (FA-8750-09-C-0179) for supporting a group to construct consensus annotations and the AMR Editor. The initial AMR bank was built under DARPA DEFT FA-8750-13-2-0045 (PI: Stephanie Strassel; co-PIs: Kevin Knight, Daniel Marcu, and Martha Palmer) and DARPA BOLT HR0011-12-C-0014 (PI: Kevin Knight).*

*Thanks to AMR annotators: aanisie, achirila, adkatz, amandamo, amorari, annsz, archna, aroman, awea, bbadarau, boconnor, bonial, brodie, canastasescu, cbobb, ebaldaeva, ebutusina, foredana, gsandru, holman, ibobaru, ierejdi, iioana, ipuiulet, isavescu, itisea, itrif, ivine, jgetman, joellis, kiragrif, kirchman, knight, laura, madalina, mduma, mfelicanu, nbrasoveanu, neilkus, omerean, palmer, ptcacenco, rporfire, schoolsh, sduman, streier, tbreiner, timjogorman, and ulf.*
