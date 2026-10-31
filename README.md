# Schooling and adolescent first birth in South Asia and adjacent countries

Code and summary results for the manuscript "Schooling and adolescent first birth in South Asia and adjacent countries: a quantitative bias analysis of retrospective birth histories from Demographic and Health Surveys" (Sahil Raiyan, Institute of Applied Statistics and Data Science, University of Dhaka).

The analysis covers seven countries: Bangladesh, India, Nepal, Pakistan, Afghanistan, Myanmar and the Maldives (16 country-surveys, women aged 20 to 29). It estimates the association between age-specific schooling and first birth before age 20 with discrete-time hazard models, pools the countries by random-effects meta-analysis, reports absolute risks, and simulates how births and marriages that end schooling could bias the estimates.

## What is in this repository

The full code is in one archive, `dhs_education_childbearing_repo_updated.zip`. Unzip it to get:

- `README.md` and `MALDIVES.md`: full instructions, script list and the order in which to run them (`MALDIVES.md` covers the seventh country and its decisions).
- Python and R scripts: country pipelines (`run_<country>.py`), pooling (`pooling.py`, `run_stage2.py`, R scripts for meta-regression and validation), and `make_seven_country_outputs.py`, which produces the manuscript tables, figures and `numbers_for_text.json`.
- `bias_analysis/`: the simulation code and the scenario grids and pooled results.
- `reference_results/`: summary results for each country and the pooled results (`stage2/`).
- `manuscript/`: LaTeX source, tables and figures of the manuscript.

## Data

The DHS individual recode files are not included, because the DHS Program does not allow redistribution. Register and request access at https://dhsprogram.com, then place the files under `data/` as described in the README inside the archive. Survey files used: Bangladesh 2014, 2017-18, 2022; India 2005-06, 2015-16, 2019-21; Nepal 2011, 2016, 2022; Pakistan 2006-07, 2012-13, 2017-18; Afghanistan 2015; Myanmar 2015-16; Maldives 2009 and 2016-17.

## Requirements

Python 3 with the packages in `requirements.txt` and R for the meta-regression and validation scripts. Bootstrap runs are slow; the archive's README gives timings.

## Results

Summary results are in `reference_results/` and `bias_analysis/`. They are enough to reproduce the pooled estimates, tables and figures without the DHS data.

## Version

This is version [v1.1.0, seven-country version]. The earlier six-country version (v1.0.0) is kept under Releases.

## Citation

Please cite the manuscript [add journal reference when available] and this archive: [new Zenodo DOI].

## Licence

MIT. See `LICENSE`.

## Contact

Sahil Raiyan, University of Dhaka, sraiyan28@isrt.ac.bd
