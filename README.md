# Description
This repository contains all new results reported in the HATCHet2 publication (in review):

* `10x`: results on the 10x CNV kit 5-sample breast tumor dataset
* `gundem`: results on the Gundem et al., 2015 multi-sample metastatic prostate cancer dataset (10 patients, 50 samples)
* `mascote-multisample`: results on MASCoTE simulated data that accompanied the original HATCHet publication (8 datasets, 32 samples)
* `mascote-singlesample`: results on MASCoTE simulated data as previous, but treating each sample as an independent dataset (32 datasets, 32 samples)
* `mirrored-simulations`: results on new simulated data featuring a high prevalence (20-30% of the genome) of mirrored-subclonal CNAs (150 datasets, 350 samples)
* `purity-simulations`: results on new simulated data featuring a range of tumor purities (191 datasets)

Code used to generate new simulated data is available in the [hatchet2-simulations repository](https://github.com/raphael-group/hatchet2-simulations/tree/main) -- `purity` and `mirrored` simulations are indicated as separate releases.
