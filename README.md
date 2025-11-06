# OnlineResults: Hand-drawn Graph Grading (CAPS)

This repo publishes the final, reproducible results for the study on *Automatic Assessment of Cartesian Graphs in the South African Context*. It evaluates **Gemini 2.5 Pro** and **GPT-4.1** across prompt styles: Zero-shot, Few-shot, Structured, Structured-Minus-Exemplar, and APE (human-in-the-loop prompt refinement) with HITL (Human In The Loop) refinements out of band.

## What’s here

- `figs/` — summary visuals used in the paper (heatmaps, grids, winner matrix, etc.).
- `Gemini_All/` — all Gemini 2.5 Pro runs, grouped by stage.  
  Each subfolder name encodes the config (group, iteration, T, top-p).
- `GPT_All/` — all GPT-4.1 runs, grouped by stage with the same naming.
- `P1_Group1_COS700/`, `P1_Group2_COS700/` — the two redraw sets used for evaluation (IDs S1–S26).
- `Exstras/` — extra showcase runs, including preview runs, GPT-5 runs, and “Gemini-2.5-flash” zero-shot dumps.


## How to verify a result quickly

1. Pick a run folder, for example:  
   `GPT_All/GPT4.1_APE_All/GPT_APE_Iteration3/Group2_All/gpt-4.1_APE_Group2_Iteration_3_Temp_0.9_topP_0.9/`
2. Open the CSVs:
   - `confusion_matrix_strict.csv`, `confusion_matrix_relaxed.csv`
   - `per_class_report_strict.csv`
   - `kappa_bootstrap.csv`
   - `all_student_marks.csv` and `per_student_appendix.csv`
3. If present, open `*_PROMPT.md` to see the exact prompt text used for that run.  
   Folder names carry `Temp_X` and `topP_Y` plus the seed where applicable.
4. Cross-check figures in `figs/` against these per-run artifacts.

## Metrics (short)

- `Acc_strict` — exact agreement with ground truth mark.
- `Acc_relaxed` — agreement within the specified acceptance set for each item.
- `kappa` variants — Cohen’s kappa (nominal and quadratic-weighted) for strict and relaxed.
- `Bias` — mean(model − expected) over items.

## Notes

- Images in `P1_*` are redraws of student-style sketches used only for evaluation.
- Runs in `Exstras/` are exploratory and not part of the main comparisons.

## License

Unless noted otherwise, the data, figures, and documentation in this repository are licensed under **Creative Commons Attribution 4.0 International (CC BY 4.0)**. You may use, share, and adapt the material with attribution and a link to the license. Please indicate if changes were made.

**Please cite:**
Charl Pieter Pretorius (2025), *Automatic Assessment of Cartesian Graphs in the South African Context*. University of Pretoria. Supervisors: Linda Marshall, Pula Rammoko, Cobus Redelinghuys. CC BY 4.0.  
License: https://creativecommons.org/licenses/by/4.0/
