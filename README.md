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

## Next steps
- Swap in a real FASTA (human mtDNA or a bacterium), tweak `window`/`step`, and re-run.
- Cite the genome source in this README.
