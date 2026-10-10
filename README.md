# Predicting General Psychopathology from Neuroimaging Data

A group project completed during **NeuroHackademy 2025** exploring the use of
neuroimaging-derived measures to predict the general psychopathology factor
(`p_factor`) in the Philadelphia Neurodevelopmental Cohort (PNC).

## Project Overview

This project used data from the
[Reproducible Brain Charts (RBC)](https://reprobrainchart.github.io/) database
to explore prediction of `p_factor`, a measure of general psychopathology.

As part of the project, we expanded the provided NeuroHackademy example
workflow to extract regional FreeSurfer-derived brain measures across multiple
cortical parcellations. The resulting dataset included regional measurements
from the PNC for subsequent exploration and predictive modeling.

The final prediction workflow used surface area from bilateral Brodmann Area 1
as features in a linear regression model trained on participants with known
`p_factor` values. The trained model was then used to generate predictions for
the held-out test participants.

## Data

Neuroimaging data were obtained through the Reproducible Brain Charts
Philadelphia Neurodevelopmental Cohort resources.

Regional measures were explored across four parcellations:

- AAL
- Glasser
- aparc.a2009s
- PALS_B12_Brodmann

Extracted FreeSurfer-derived measures included cortical surface area,
gray-matter volume, cortical thickness, curvature, folding, and related
regional measurements.

## Repository Contents

- `analysis.ipynb` — prediction workflow and generation of held-out predictions
- `extract_data.ipynb` — extraction of regional neuroimaging measures
- `allSubs_brainmeasures.csv` — compiled participant-level brain measures
- `data/` — extracted regional measurements
- `results/group5.tsv` — predictions generated for the held-out test set

## Contributors

This project was completed collaboratively by:

- Samantha K. Eaton
- G. Lynn Kurteff, PhD
- Jamie Mitchell
- Additional members of NeuroHackademy 2025 Group 5

## Acknowledgments

This project was completed during
[NeuroHackademy 2025](https://neurohackademy.org/).

The original project template and example workflow were developed by
Noah C. Benson and the NeuroHackademy team.
