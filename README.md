[![DOI](https://zenodo.org/badge/555768615.svg)](https://zenodo.org/badge/latestdoi/555768615)
# RNAChallenge dataset 

The dataset is derived from publicly available datasets used for the classification of protein-coding and non-coding RNAs through a large scale benchmark of tools. It is a challenging validation dataset containing hard instances only and it serves dual purpose:
1. Standard test dataset to evaluate the performance of tools is essential for developing more accurate and less biased models for correct annotation of transcripts, but such datasets were not present until now. Additionally, best and least performing models in a benchmark under and over-fit this dataset respectively. So, comparing the models on RNAChallenge dataset helps to evaluate tools precisely.
2. The misannonation of transcripts is a well-known problem in the biology domain that needs to be addressed. This dataset provides the opportunity to recognize the false positive and negative instances through automated approaches and bioinformatics experts.

## Source
We have collected 135 small and large transcriptomic datasets covering 49 species for a large scale benchmark of existing tools. Most of these datasets were acquired at the species level covering animal, plant, and fungi kingdoms while a few datasets gathered sequences from multiple species. The details about these datasets are as follows:

<img src="/image/Figure.png" width="800">

(A) The kingdom wise coverage of species and heterogeneous datasets, (B) share of mRNAs and ncRNAs and (C) balanced and imbalanced datasets. (D) Taxonomic distribution of species at kingdom level and heterogeneous datasets at their primary level and (E) Length distribution of sequences at species, subphylum, class, kingdom, and domain levels.

## Building dataset
The classification decisions of 48 models are averaged to obtain the classification confidence score for each instance. The sequences less than the specified threshold are filtered out and duplicate sequences are removed with CD-HIT tool to build the dataset. The threshold of accurate classifications by at most 8 models has been used for constructing the ***RNAChallenge*** dataset. This test set contains 16,243 mRNAs and 11,040 ncRNAs belonging to species from animal, plant, and fungi kingdoms.

## Reference
When using this dataset in your work, please cite our paper:

*It will be updated soon.*
