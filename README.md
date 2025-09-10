# The Impact of Apportionment Methods on Political Representation: A Comparative Analysis of Spain’s Electoral System

This repository contains the full code developed for my Master Thesis in Computational Social Science at Universidad Carlos III de Madrid. The project analyses the proportionality of the Spanish electoral system, combining historical election data with simulations of alternative institutional rules.

The final written document can be found in the PDF file Master Thesis.pdf

## Contents

- Data preparation: data extracted from {pollspain} via summary_election_data(), which retrieves aggregate electoral results for a given contest and aggregation level.
- Disproportionality indices: implementation of standard measures (Gallagher, Loosemore–Hanby, Rae, Lijphart, Sainte-Laguë, etc.) applied to Spanish elections.
- Apportionment methods: functions to allocate seats under different formulas (D’Hondt, Webster, Adams, Hamilton, Hagenbach–Bischoff, Hill, Dean and FPTP).
- Simulations across elections (1982-2023):
  - Threshold effects (0–10%)
  - Constituency designs (provincial, regional, national)
  - Apportionment methods
  - Robustness analysis with Dirichlet-based vote perturbations
- Visualization: scripts to generate all figures included in the thesis (evolution of disproportionality indices, seat reallocations, robustness comparisons, etc.).

## Requirements

- R (≥ 4.3)
- Main packages: pollspain, tidyverse, MCMCpack, stringr.

##  Reproducibility

All results are fully reproducible by running the R Markdown files in order:

- Disproportionality study: run Main Analysis.Rmd (data import via summary_election_data(), generation of indices and apportionment methods, simulations across elections, and main figures for thresholds ×  constituencies × methods).
- Robustness analysis: run Robustness Analysis.Rmd (Robustness analysis with Dirichlet-based vote perturbations).
