# Catalogues of LISA-detectable sBHB inspirals and confusion backgrounds following the GWTC-3 fiducial model posterior

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13974091.svg)](https://doi.org/10.5281/zenodo.13974091)

## Data set

The contents of `SNR_min_2_z1_LISA_SNR.tar.gz` (see Zenodo DOI image link above) consist of approximately 10k folders, each corresponding to each of the samples of the public GWTC-3 fiducial sBHB population model posterior, and containing the following files:

- `population.yaml`: population parameters of this sample.
- `background.txt`: frequencies and characteristic strain squared of the sBHB confusion noise in the LISA band for this population.
- `population_detector_frame_SNR.h5`: subset of loud sBHB sources, including but not limited to those with LISA SNR larger than 4 (missing in some samples). 

For a description of the population parameters in `population.yaml` and the individual source parameters in `population_detector_frame_SNR.h5`, see the contents of the `Demo.ipynb` notebook.

To be able to run the notebooks described below, uncompress the `SNR_min_2_z1_LISA_SNR.tar.gz` file inside a `data/` subfolder under that of the notebook.

## Demo notebook

For examples of how to load and process the catalogues, see the `Demo.ipynb` notebook.

This notebook requires the following Python packages:

    numpy, scipy, pandas, matplotlib, pyyaml, tqdm
    
Some of the plots in the notebook require the `extrapops` simulation package:

    $ git clone git@github.com:JesusTorrado/extrapops.git
    $ cd extrapops
    $ pip install .

## References

For details, see, and cite accordingly:

#### Individual sources:

*Stellar-mass black-hole binaries in LISA: characteristics and complementarity with current-generation interferometers*,<br>
R. Buscicchio, J. Torrado, C. Caprini, G. Nardini, N. Karnesis, M. Pieroni, A. Sesana
Submitted to JCAP, [arXiv:2410.18171 [astro-ph.HE]](https://arxiv.org/abs/2410.18171)

#### Confusion background:

*Stochastic gravitational wave background from stellar origin binary black holes in LISA*,<br>
S. Babak, C. Caprini, D. G. Figueroa, N. Karnesis, P. Marcoccia, G. Nardini, M. Pieroni, A. Ricciardone, A. Sesana, J. Torrado<br>
[JCAP 08 (2023) 034](https://iopscience.iop.org/article/10.1088/1475-7516/2023/08/034), [arXiv:2304.06368 [astro-ph.CO]](https://arxiv.org/abs/2304.06368)

## Questions and comments

Please use the [GitHub issue tracker](https://github.com/JesusTorrado/LISA_sBHB_catalogues/issues) or contact the corresponding authors of the papers above.
