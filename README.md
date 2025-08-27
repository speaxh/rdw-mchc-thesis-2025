# RDW:MCHC — Thesis Code (MIMIC-IV & eICU)

This repository contains the code used in my MRes thesis analysing the RDW:MCHC ratio
for early risk stratification in critical care.

## What’s here
- `all_the_code.ipynb`: end-to-end notebook (outputs cleared).
- `src/`: modular Python scripts mirroring the notebook.
- `sql/`: key DuckDB queries for cohort and first-24h extraction.
- `docs/data_flow.pdf`: 1-page pipeline diagram.
- `sample_data/`: tiny synthetic examples to illustrate inputs only.

## Reproducibility
Due to licence restrictions, **raw MIMIC-IV/eICU data are not included**.
To reproduce:
1. Obtain access to MIMIC-IV/eICU.
2. Update paths in the notebook or `src/utils.py`.
3. Create the environment:  
   `pip install -r requirements.txt`  
   *or* `conda env create -f environment.yml && conda activate rdw-mchc`
4. Run the notebook or execute the scripted pipeline.

## Environment
See `requirements.txt` (or `environment.yml`) for pinned versions.

## Licence
MIT (see `LICENSE`).
