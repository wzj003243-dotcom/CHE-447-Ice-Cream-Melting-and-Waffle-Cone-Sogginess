# CHE447 Ice Cream Cone Project

Physics-based and data-driven study of ice cream melting and cone sogginess.

## Repo structure

- `data/`
  - main Excel template
  - cleaned CSV exports for modeling
- `docs/`
  - proposal
  - heat section writeup
  - sogginess section writeup
- `notebooks/`
  - sklearn / analysis notebooks
- `models/`
  - COMSOL model link or one approved master model only
- `results/`
  - exported plots, tables, and final figures

## What should go in this repo

Recommended:
- final Excel template
- final cleaned dataset CSV
- notebooks
- SOP / notes
- final report source files

Avoid committing:
- COMSOL temporary lock files such as `~model*.mph`
- multiple duplicate `.mph` case files
- very large videos
- random duplicate Excel files

## Suggested workflow

1. Keep one approved COMSOL master model.
2. Run each case and enter results into the main Excel template.
3. Export a cleaned CSV for machine learning.
4. Run the sklearn notebook.
5. Save final plots in `results/`.

## Current modeling outputs

Main targets:
- `t_melt_onset_s`
- `t_noticeable_soggy_s`
- `t_unacceptably_soggy_s`
- `t_finish_s`
- `M_melt_1800s_g`
- `M_abs_1800s_g`
- `SI_1800`

## Notes for team members

- `t_melt_onset` is case-specific and must be recalculated for each case.
- `dH_melt` is a post-processing parameter and does not have to be inside COMSOL.
- Keep parameter names consistent across the Excel template and notebooks.
