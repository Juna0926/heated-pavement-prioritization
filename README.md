# Risk-Based Prioritization of Heated-Pavement Deployment in Gwangjin-gu

> A public-data machine-learning workflow for prioritizing roads where heated-pavement installation could reduce winter road-risk exposure.

**Project:** 2025 Gwangjin-gu Big Data Analysis Competition  
**Core method:** Random Forest · probability ranking · road-level contextual review

---

## Problem

Heated pavement can reduce winter hazards such as snow / ice-related road risk, but installation resources are limited. The project therefore reframed deployment as a **road-prioritization problem**: use public data to identify road segments with characteristics associated with higher installation priority, then review the highest-ranked candidates in their actual road context.

## Analytical workflow

1. Collect and preprocess Gwangjin-gu public datasets related to road / winter-risk conditions.
2. Engineer road-level explanatory variables.
3. Train and evaluate a **Random Forest** classifier.
4. Use predicted `RF_probability` to rank candidate roads.
5. Select the top five candidate roads.
6. Review candidate geometry / surrounding context rather than relying on model probability alone.

## Model result

![Random Forest AUC](assets/figure-01-random-forest-auc.svg)

The competition report presents a **Random Forest AUC of 0.888**.

## Candidate prioritization

![Top five candidate roads](assets/figure-02-top-five-roads.svg)

The final analysis ranked five roads by Random Forest installation probability and then reviewed each candidate using street / road context.

## Expected impact & limitations

![Expected impact](assets/figure-03-expected-impact.svg)

The project positioned the model as a transparent screening tool that could support more efficient deployment and later extension to related winter-road infrastructure decisions.

The report explicitly notes limitations including:

- Different update cycles across public datasets, which can introduce time mismatch
- Possible coordinate / spatial error after preprocessing
- Limited availability of detailed road-width / road-environment information
- Imbalance in road-type representation within the available data

These limitations are important: the ranking is a decision-support result, not a substitute for engineering inspection or municipal feasibility review.

## Project outputs

- [`outputs/heated-pavement-analysis-public-excerpt.pdf`](outputs/heated-pavement-analysis-public-excerpt.pdf) - concise public-safe technical excerpt derived from the competition report.
- [`outputs/PROJECT_OUTPUTS.md`](outputs/PROJECT_OUTPUTS.md) - source provenance, top-road ranking, and public-release notes.

---

**Junha Won** · Ajou University  
[Portfolio](https://juna0926.github.io/Portfolio/) · [GitHub](https://github.com/Juna0926)
