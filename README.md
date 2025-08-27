# GC Content + Sliding Window (Publishable Mini-Project)

**Updated:** 2025-08-26

## Goal
Compute overall GC% and a sliding-window GC profile for a DNA sequence (FASTA), then save figures and tables that others can reuse.

## Methods (brief)
- **Overall GC%** = (count of G or C) / (count of A/C/G/T) × 100.
- **Sliding windows**: walk along the sequence in fixed-size windows and compute GC% per window.

## Results (quick look)
**Overall GC%:** 50.0%

GC% profile:

![GC profile](figures/gc_profile.png)

Overall GC% bar:

![Overall GC](figures/gc_overall.png)

First few windows:

| start | end | length | gc_percent |
|---:|---:|---:|---:|
| 0 | 200 | 200 | 50.0 |
| 100 | 300 | 200 | 50.0 |
| 200 | 400 | 200 | 50.0 |
| 300 | 500 | 200 | 50.0 |
| 400 | 600 | 200 | 50.0 |


## Next Steps
We extended the analysis by running the pipeline on **real FASTA sequences**:
- Human mitochondrial genome (rCRS, NC_012920.1)
- *Escherichia coli* K-12 MG1655 (NC_000913.3)

This produced updated GC% profiles and tables in the `results/` folder.

## Data Sources
- **Human mitochondrion (rCRS)** — NCBI RefSeq **NC_012920.1**  
  FASTA viewer: https://www.ncbi.nlm.nih.gov/sviewer/viewer.fcgi?id=NC_012920.1&db=nuccore&report=fasta
- **Escherichia coli K-12 substr. MG1655** — NCBI RefSeq **NC_000913.3**  
  FASTA viewer: https://www.ncbi.nlm.nih.gov/sviewer/viewer.fcgi?id=NC_000913.3&db=nuccore&report=fasta

*This section was appended on 2025-08-27 to cite sequence sources used in analyses.*
