# Explore the Alphafold low confidence prediction

## Introduction

This repository is to collect and select the AlphaFold predictions, which have < 70 confidence across all the residuals. Then mapping the AlphaFold id as follows:

AlphaFold -> Uniprot -> PDB -> SCOPe. Ideally, we would like to find a set of domains,  which AlphaFold couldn't make predictions, but we have human annotation already.

I implemented the mapping function but did not find many target domains. More specifically, only [a few low confidence human domains](https://docs.google.com/presentation/d/1ZNDjIBrRfZolcPODRHFBYb38hdytWTVMn6Sca1CfCAU/edit?usp=sharing) can be mapped to PDB, and only 4 of them have SCOPe fold annotation. I also tried C.elegans, Rat, Mouse, Drosophila, and Zebrafish. But neither of them has an entity in PDB. (I feel a bit confused about this part, though).

I will stop here for now. But there could be more domains if I change the definition of misprediction (currently, it is < 70 across all residuals).