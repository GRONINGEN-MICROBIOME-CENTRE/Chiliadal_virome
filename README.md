# Comprehensive profiling of infant gut virome assembly reveals associations with eczema and wheeze

This repository contains the scripts used for the data analysis in the study:

**“Comprehensive profiling of infant gut virome assembly reveals associations with eczema and wheeze”** (available on bioRxiv).

---

## Table of Contents

- [Summary](#summary)
- [Cohort](#cohort)
- [Code Overview](#code-overview)
- [Data Availability](#data-availability)
- [System Requirements](#system-requirements)
- [Installation and Runtime](#installation-and-runtime)
- [Citation](#citation)
- [Contact](#contact)

---

## Summary

XXX

---

## Cohort

This study is based on the **Lifelines NEXT (LLNEXT)** cohort, a large, prospective, population-based birth cohort in the Netherlands designed to investigate early-life determinants of health and disease.

- Cohort overview and data catalogue:  
https://umcgresearchdatacatalogue.nl/all/cohorts/LIFELINES_NEXT  

- Original cohort description:  
https://pubmed.ncbi.nlm.nih.gov/32100173/

---

## Code Overview

### 1. Upstream Analysis
**Location:** [`01.Upstream_analysis`](https://github.com/GRONINGEN-MICROBIOME-CENTRE/Chiliadal_virome/tree/main/01.Upstream_analysis)
**Location:** ``

This section contains scripts for raw data processing up to the generation of RPKM tables.

The folder contains a README with detailed instructions.

---

### 2. Downstream Analysis
**Location:** [`02.Downstream_analysis`](https://github.com/GRONINGEN-MICROBIOME-CENTRE/Chiliadal_virome/tree/main/02.Downstream_analysis)

This section contains scripts for:

- Metadata processing  
- Virus characterization  
- Statistical analysis  
- Figure generation  

Scripts are organized into analysis-type-specific subfolders.

Each folder includes a README with further details.

---

## Data Availability

Sample information, timepoints, clinical metadata, family structure, and quality-trimmed, human-contaminant-free metagenomic and VLP sequencing reads are available in the **European Genome-phenome Archive (EGA)** under study IDs:

- EGAS50000000133  

Additional source data, including redundant viral sequences, the NEXT virome catalog, and associated metadata, are available via [**FigShare**](https://doi.org/10.6084/m9.figshare.32685267 ).

For reproducibility, we recommend using the full FigShare dataset for downstream analyses.

For upstream analyses, any subset of samples from the original study can be used. Outputs may vary depending on the selected subset, but should converge on the same set of identified viruses and associated metadata.

The reference output is available in the `NEXT_virome_catalog` folder.

---

## System Requirements

A complete list of software tools and package versions is provided in the Methods section of the associated bioRxiv manuscript.

Some analyses can be run on a standard laptop, but computationally intensive steps require HPC resources for practical runtimes.

All analyses were performed on the **Hábrók high-performance computing cluster**, provided by the Genomics Coordination Center and the Center for Information Technology at the University of Groningen.

---

## Installation and Runtime

Before running the code, install all required dependencies following the documentation for each tool or package.

- **Installation time:** typically within one day, depending on system setup  
- **Runtime:**
  - Upstream analysis: variable (see `.sh` script headers for estimates)
  - Downstream analysis: typically a few hours  

---

## Citation

If you use this repository, please cite both the publication and the data resources.

**Publication:**  


**Data resource:**  
https://doi.org/10.6084/m9.figshare.32685267

---

## Contact

For questions about the analysis workflow or datasets, please open an issue or contact:

**Sanzhima Garmaeva**  
📧 sana.garmaeva@gmail.com
