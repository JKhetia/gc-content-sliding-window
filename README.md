# GC Content + Sliding Window 

**Updated:** 2025-08-26

A simple Jupyter notebook that computes **overall GC%** and **sliding-window GC profiles** from any FASTA file — a staple in **genome QC** and exploratory analysis.

Use it as a template to learn bioinformatics while producing **publishable** figures and CSVs.

## Methods (brief)
- **Overall GC%** = (count of G or C) / (count of A/C/G/T) × 100.
- **Sliding windows**: walk along the sequence in fixed-size windows and compute GC% per window.

## Results (quick look)
**Overall GC%:** 50.0%

GC% profile:

![GC profile](gc_profile.png)

Overall GC% bar:

![Overall GC](gc_overall.png)

First few windows:

| start | end | length | gc_percent |
|---:|---:|---:|---:|
| 0 | 200 | 200 | 50.0 |
| 100 | 300 | 200 | 50.0 |
| 200 | 400 | 200 | 50.0 |
| 300 | 500 | 200 | 50.0 |
| 400 | 600 | 200 | 50.0 |

## Next steps
- Swap in a real FASTA (human mtDNA or a bacterium), tweak `window`/`step`, and re-run.
- Cite the genome source in this README.
