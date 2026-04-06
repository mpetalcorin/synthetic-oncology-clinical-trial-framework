# synthetic-oncology-clinical-trial-framework
A synthetic, literature-informed oncology clinical trial workflow that transforms simulated patient data into SDTM-like and ADaM-like datasets, publication-style analyses, and decision-oriented translational insights.
<img width="1520" height="965" alt="Screenshot 2026-04-06 at 15 46 56" src="https://github.com/user-attachments/assets/914eb6bd-2128-4a5e-87a8-0c20af2fed62" />
# Synthetic Oncology Clinical Trial Framework

## Overview
This repository presents a synthetic, literature-informed oncology clinical trial workflow designed to demonstrate an end-to-end clinical data science pipeline for translational oncology. The project follows the sequence **Patient → Data → Dataset → Analysis → Tables/Figures → Decision** and integrates simulated patient-level clinical, biomarker, exposure, tumor, safety, and survival data into standardized and analysis-ready datasets.

The workflow was developed as a methodological and portfolio demonstration. It does not contain real patient records and does not represent the results of an actual clinical trial. Instead, it reproduces a biologically plausible and analytically coherent efficacy-safety signal structure inspired by common patterns reported in peer-reviewed oncology studies.

## Project Objectives
The main objectives of the project are:
1. To simulate a realistic phase II randomized oncology trial dataset.
2. To transform raw data into SDTM-like and ADaM-like structures.
3. To perform survival, tumor, biomarker, exposure-response, and safety analyses.
4. To generate publication-style tables and figures.
5. To support decision-oriented interpretation relevant to oncology drug development.

## Repository Structure
- `01_simulate_raw_data.ipynb`  
  Simulates raw patient-level source datasets including demographics, visits, exposure, labs, tumor assessments, biomarkers, adverse events, concomitant medications, and survival.
- `02_create_sdtm_dm_sv_ex.ipynb`  
  Builds SDTM-like DM, SV, and EX domains.
- `03_create_sdtm_lb_tu_ae_cm.ipynb`  
  Builds SDTM-like LB, TU, AE, and CM domains.
- `04_create_adsl_corrected.ipynb`  
  Creates the subject-level analysis dataset, ADSL.
- `05_create_adtte_corrected.ipynb`  
  Creates the time-to-event analysis dataset, ADTTE.
- `06_create_adlb_adtu_adbm_adae_corrected.ipynb`  
  Creates ADLB, ADTU, ADBM, and ADAE.
- `07_generate_tables_corrected.ipynb`  
  Generates publication-style tables.
- `08_survival_analysis_corrected_v2.ipynb`  
  Generates Kaplan-Meier plots, subgroup analyses, and survival summaries.
- `flagship_oncology_patient_data_dataset_analysis_decision.ipynb`  
  Integrates the full workflow into a single flagship analysis notebook.

## Core Datasets
### Raw source datasets
- `demographics_raw.csv`
- `visits_raw.csv`
- `exposure_raw.csv`
- `labs_raw.csv`
- `tumor_raw.csv`
- `biomarker_raw.csv`
- `adverse_events_raw.csv`
- `conmeds_raw.csv`
- `survival_raw.csv`

### SDTM-like datasets
- `DM.csv`
- `SV.csv`
- `EX.csv`
- `LB.csv`
- `TU.csv`
- `AE.csv`
- `CM.csv`

### ADaM-like datasets
- `ADSL.csv`
- `ADTTE.csv`
- `ADLB.csv`
- `ADTU.csv`
- `ADBM.csv`
- `ADAE.csv`

## Main Analyses
The workflow supports the following analyses:
- Baseline characteristics by treatment arm.
- Treatment exposure and dose intensity.
- Best overall response and clinical benefit.
- Kaplan-Meier overall survival and progression-free survival.
- Subgroup hazard ratio exploration.
- Longitudinal tumor burden and ctDNA analysis.
- Exposure-response analysis.
- Adverse event and safety analysis.
- Publication-ready tables, figures, and manuscript outputs.

## Key Outputs
### Tables
- Baseline demographic and disease characteristics.
- Treatment exposure and dose intensity.
- Best overall response.
- Adverse event summary.
- Key laboratory parameters over time.
- Biomarker change over time.
- Survival summary.
- Overall survival subgroup hazard ratios.

### Figures
- Kaplan-Meier overall survival.
- Kaplan-Meier progression-free survival.
- Forest plot of subgroup hazard ratios.
- Mean tumor percent change over time.
- Waterfall plot of best tumor response.
- Spider plot of tumor trajectories.
- ctDNA change over time.
- Exposure-response plot.
- Adverse event frequency by treatment arm.
- Conceptual graphical summary figure.

## Scientific Scope
This project focuses on the integration of:
- Radiographic tumor response.
- Circulating tumor DNA dynamics.
- Systemic inflammation markers.
- Immune and proliferation biomarkers.
- Exposure and dose intensity.
- Safety and treatment tolerability.
- Survival outcomes.

The resulting outputs are intended to resemble the kind of evidence package used in translational oncology and early clinical development.

## Important Note
All results are based on synthetic, literature-informed data generated for methodological demonstration, portfolio development, and reproducible analytics workflow design. No real patient-level clinical trial data are included.

## Suggested Uses
This repository may be useful for:
- Clinical data science portfolio demonstration.
- Oncology analytics workflow prototyping.
- SDTM and ADaM dataset practice.
- Survival and longitudinal modeling exercises.
- Publication-style figure and table generation.
- Internal training in translational oncology analytics.

## Software
The workflow was implemented in Python using Jupyter notebooks and common scientific libraries, including:
- `numpy`
- `pandas`
- `matplotlib`
- `lifelines`
- `reportlab`
- `python-docx`

## Reproducibility
All major steps were structured as notebooks so that raw data generation, dataset creation, analysis, table generation, figure production, and manuscript assembly can be reproduced in sequence.

## License and Data Use
Because the data are synthetic, this project is intended for educational, methodological, and demonstration purposes. Users should clearly state that the outputs are synthetic if figures, tables, or derivative analyses are reused.

## Citation
**Petalcorin, M.I.R.** (2026). An End-to-End Synthetic Oncology Clinical Trial Framework Integrating Radiographic Response, Circulating Tumor DNA, Safety, and Survival for Decision-Oriented Clinical Data Science. https://github.com/mpetalcorin/synthetic-oncology-clinical-trial-framework


