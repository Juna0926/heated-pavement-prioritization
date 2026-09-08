# Risk-Based Prioritization of Heated Pavement Deployment

> A spatial machine-learning framework for prioritizing road segments for heated-pavement installation using road, accident, weather, and facility data.

**Period:** May. 2025  
**Domain:** Spatial data analysis · Public safety  
**Core methods:** Random Forest · PCA · KD-Tree  
**Output:** Ranked candidate road segments for heated-pavement deployment

---

## Overview

Heated pavement can reduce winter road hazards, but installation resources are limited. This project therefore framed deployment as a **risk-based prioritization problem**: integrate heterogeneous public datasets, construct road-level spatial features, estimate relative installation priority, and rank candidate road segments for decision support.

The workflow combined road, accident, weather, and nearby-facility information and used spatial preprocessing together with machine learning to convert multiple risk signals into a transparent prioritization result.

## Data integration

The analysis combined public datasets related to:

- Road characteristics
- Traffic / accident information
- Weather and winter-risk conditions
- Nearby facilities and contextual infrastructure
- Spatial coordinates and road-segment relationships

## Spatial preprocessing

The project used **PCA** and **KD-Tree**-based processing to organize heterogeneous spatial variables and map contextual information to road-level analysis units.

The goal was to transform multiple datasets with different scales and coordinate structures into a consistent feature space for road-priority modeling.

## Modeling workflow

1. Collect and preprocess road, accident, weather, and facility data.
2. Construct road-level explanatory variables.
3. Apply spatial preprocessing and feature construction using **PCA** and **KD-Tree**.
4. Train a **Random Forest** model for relative installation-priority estimation.
5. Rank candidate road segments using model probability.
6. Review the highest-ranked roads in their actual spatial context.

## Main result

![Random Forest AUC](assets/figure-01-random-forest-auc.svg)

The competition-stage analysis reported a **Random Forest AUC of 0.888**.

The final workflow converted model output into a ranked list of road segments rather than treating prediction as an automatic installation decision.

## Candidate prioritization

![Top five candidate roads](assets/figure-02-top-five-roads.svg)

The analysis identified the highest-priority candidate roads and then reviewed their geometry and surrounding context to support a more interpretable deployment recommendation.

## Expected impact & limitations

![Expected impact](assets/figure-03-expected-impact.svg)

The project demonstrates how spatial machine learning can support allocation of limited infrastructure resources. The ranking should be interpreted as a **screening / decision-support result**, not as a substitute for engineering inspection or municipal feasibility review.

Important limitations include:

- Different update cycles across public datasets
- Potential coordinate / spatial matching error
- Limited availability of detailed road-width and road-environment information
- Imbalance in road-type representation

## Public outputs

- [`outputs/heated-pavement-analysis-public-excerpt.pdf`](outputs/heated-pavement-analysis-public-excerpt.pdf) - concise public-safe technical excerpt derived from the competition report.
- [`outputs/PROJECT_OUTPUTS.md`](outputs/PROJECT_OUTPUTS.md) - source provenance, top-road ranking, and public-release notes.

---

**Junha Won** · Ajou University  
[Portfolio detail](https://juna0926.github.io/Portfolio/projects/gwangjin.html) · [Portfolio](https://juna0926.github.io/Portfolio/) · [GitHub](https://github.com/Juna0926)
