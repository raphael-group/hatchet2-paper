HATCHet is an algorithm to infer haplotype- and clone-specific copy-number aberrations (CNAs), clone proportions, and whole-genome duplications (WGD) for several tumor clones jointly from one or more bulk tumor samples from the same patient. HATCHet2 is implemented in the HATCHet repository (versions 1.1+): https://github.com/raphael-group/hatchet

# Overview
This repository contains supporting data for the results that accompany the HATCHet2 paper. It contains HATCHet2 results on the following datasets:
* `hatchet2-sim-results`: MASCoTe simulated datasets from the [original HATCHet paper](https://www.nature.com/articles/s41467-020-17967-y) (available in the [HATCHet publication repository](https://github.com/raphael-group/hatchet-paper))
* `gundem`: 50 whole-genome sequencing samples in total from 10 patients with prostate cancer from the Gundem et al., 2015 study. Data availability is described in the [original publication](https://www.nature.com/articles/nature14347).
* `10x`: m10x Genomics single-cell breast cancer dataset: about 10500 cells total from low-coverage single-cell whole-genome sequencing from 5 sections of a breast tumor. Described in an [application note on the 10x website](https://pages.10xgenomics.com/rs/446-PBO-704/images/10x_AN026_SCCNV_Assessing_Tumor%20Heterogeneity_digital.pdf).

This repository also contains HATCHet results on the MASCoTe simulated data in `hatchet-sim-results`, run with parameters set to match HATCHet2 as closely as possible.

# Directory contents
Each directory corresponding to a single individual contains:
* `results`: contains results reported at the bin level (`best.bbc.ucn`) and also concatenated into segments after the fact (`best.seg.ucn`). The columns in these tables are described in detail in the HATCHet2 software documentation: http://compbio.cs.brown.edu/hatchet/doc_compute_cn.html
* `summary`: contains various visualizations of the results, described in detail in the HATCHet2 software documentation: http://compbio.cs.brown.edu/hatchet/doc_plot_cn.html
* `hatchet.ini`: contains the parameters needed to fully specify a run of HATCHet2 (or a run of HATCHet using backwards compatibility settings to access the older modules). See the HATCHet2 documentation for more details on how to use this file to run HATCHet2: http://compbio.cs.brown.edu/hatchet/examples/demo-complete/demo-complete.html
