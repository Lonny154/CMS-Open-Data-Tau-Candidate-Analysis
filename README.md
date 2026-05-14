# CMS Open Data Tau Candidate Analysis

## Overview

This project explores reconstructed tau candidates from CERN CMS Open Data using Python. 
The dataset is provided in NANOAOD format, which allows analysis with common Python tools such as `uproot` and `awkward` arrays.

The goal of this project was to perform an exploratory analysis of tau candidate features and compare all reconstructed tau candidates against stronger tau-like candidates selected using a DeepTau tau-vs-jet score threshold.

## Tools Used

- Python
- Jupyter Notebook
- uproot
- awkward arrays
- pandas
- matplotlib
- CMS Open Data

## Dataset

This project uses public CMS Open Data from the CERN Open Data Portal.

Dataset: Tau primary dataset in NANOAOD format from RunH of 2016  
DOI: 10.7483/OPENDATA.CMS.TTK7.008J

## Analysis

The analysis focused on three tau candidate variables:

- `Tau_pt`: tau transverse momentum
- `Tau_eta`: tau pseudorapidity
- `Tau_rawDeepTau2017v2p1VSjet`: DeepTau tau-vs-jet discriminator score

A threshold of:

```python
Tau_rawDeepTau2017v2p1VSjet > 0.8
