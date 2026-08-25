# Dungeness Crab Cohort Biomass Modeling

This project uses mathematical modeling to compare candidate models for **Dungeness crab cohort biomass** across 52 yearly time steps. The goal was to determine which model best represented the observed biological growth and decline, evaluate its performance, and use the selected model to examine longer-term behavior.

Developed as part of **MATH 440: Mathematical Modeling** at Christopher Newport University.

## Project Overview

The analysis follows a model-selection workflow rather than relying on a single assumed model. Candidate models are fit to the observed biomass data and compared quantitatively before the strongest model is evaluated further.

The project includes:

- fitting multiple candidate mathematical models to biological data
- parameter estimation and regression modeling
- model comparison using **AIC** and **AICc**
- residual analysis
- holdout validation
- forecasting with the selected model
- interpretation of growth, decline, and long-term cohort behavior

## Methods

The workflow emphasizes both model fit and validation. AIC/AICc are used to compare candidate models while accounting for model complexity, followed by residual analysis and a holdout test to evaluate how well the selected model generalizes beyond the data used for fitting.

## Repository Contents

- `dungeness_crab_biomass_modeling.ipynb` — complete analysis and modeling workflow
- `data/DS14.csv` — dataset used in the project
- `figures/` — model comparison, residual, validation, and forecast figures

## Skills Demonstrated

- Mathematical modeling of a biological system
- Parameter estimation and model selection
- Quantitative model validation
- Scientific computing in Python
- Data visualization and interpretation
- Translating a real-world biological problem into a testable mathematical framework

## Context

This project is part of my broader interest in using applied mathematics and computation to understand real physical and biological systems. I am particularly interested in extending these skills toward biomedical engineering, biomechanics, and physiological modeling.
