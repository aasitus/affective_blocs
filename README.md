# Analyzing affective polarization with FNES data_2003

This repository contains code for analyzing affective polarization and affective blocs in Finland using data from the 2007 to 2019 Finnish National Election Studies. The code can be used to replicate the analysis in the following publication:

Kekkonen, Arto & Ylä-Anttila, Tuomas (2021). Affective blocs: Understanding affective polarization in multiparty systems. SocArXiv. [url]

Please cite the publication if you find this useful!

The code should be combined with data from [FNES](https://www.vaalitutkimus.fi/en). Do note that we used an unpublished version of the 2019 data, and there may be slight differences in the published data which mean that the code does not produce an exact replication of the results in the paper. If you notice any major differences, please let me know.

## Contact information

arto.kekkonen@iki.fi

## Instructions

This combines Python and R code in Jupyter and R notebooks. The notebooks can be used for exploration as well as to output tables (as CSV files) and plots. Here's how to use this:

1. Set the data and plot path variables at the beginning of each notebook.
2. Run the Jupyter notebook block by block. This computes the affective polarization index for each survey year, and writes the inter-party rating and distance matrices in CSV files.
3. Run the R_plotting R notebook block by block. This takes the matrices from the previous step and uses them to create heatmaps.
4. Run the lpa R notebook block by block. This creates latent profile analysis (Gaussian finite mixture) models from party thermometers and outputs related plots used in the paper and its appendix, and can also be used to investigate additional models.

Some blocks can take a while to run in steps 2 and 3.
