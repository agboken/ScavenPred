# ScavenPred and ACE-iPred reproducibility materials

These files support the revised ScavenPred/ACE-iPred manuscript submitted to *Bioinformatics Advances*.

## Public code inventory

- [Original ScavenPred development notebook](../Scavenpred.ipynb): the historical development notebook already in this public repository.
- [ScavenPred complete analysis notebook](notebooks/ScavenPred_complete_training_and_analysis.ipynb): displays the saved data-curation, training-only screening, VIF, wrapper-selection, tuning, held-out evaluation and SHAP results in the research reproducibility package. This **is not** an independently executable implementation of every feature-selection step.
- [ACE-iPred complete training and analysis notebook](notebooks/ACE_iPred_complete_training_and_analysis.ipynb): code for fitting and evaluating the frozen Random Forest using the cleaned feature matrices and independent-test dataset from the research package.

The two newer notebooks were copied from the research archive with execution outputs removed to keep the code legible. Historical provenance and results should be distinguished from a fresh successful rerun.

## Model configurations

ScavenPred final descriptors: `E5`, `ProtFP3`, `BLOSUM6`, `BLOSUM3`, `Z3`.

ACE-iPred final descriptors: `BLOSUM4`, `BLOSUM1`, `KF5`, `VHSE2`, `BLOSUM10`, `SVGER2`, `SVGER3`, `ProtFP7`, `SVGER4`, `MSWHIM3`.

## Data and verification status

**Incomplete public reproduction (as of 10 November 2026):** The versioned full data/outputs archive contains training and independent-test feature matrices, cleaned/overlap-audited datasets, univariate screening, VIF and wrapper-selection tables, hyperparameter optimisation, SHAP and evaluation reports. The archive has **not yet been fully uploaded to this public repository**. These notebooks depend on those files and cannot yet independently reproduce the entire analysis from a clean clone.

In particular, the saved selection tables are not a substitute for executable, fold-contained feature-selection scripts. Reproduction of the manuscript's leakage-control claims will require those corrected scripts and a fresh-run audit.

Do **not** interpret any published notebook as proof that leakage is eliminated without independently rerunning its preprocessing, feature-selection and evaluation pipeline.

## Public web predictors

- [ScavenPred](https://pepsilico.com/tools/scavenpred/)
- [ACE-iPred](https://pepsilico.com/tools/ace-ipred/)

These prediction services do not substitute for independent experimental reproduction.

## Research separation and intellectual property

SAPIEN-Pep and SIPPAD are a separate protected research programme and are not included in this research release.
