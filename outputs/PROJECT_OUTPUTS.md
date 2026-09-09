# Public Project Outputs

## Source artifact reviewed

- `2025 광진구 빅데이터 분석 공모전 - 광진구 열선 설치 우선 도로 예측 ML 모델 생성` analysis report.

## Current authoritative framing

The current README and Portfolio frame the project as a **risk-based infrastructure prioritization** workflow:

**road + accident + weather + facility data → PCA / KD-Tree spatial preprocessing → Random Forest risk score → heated-pavement deployment priority**.

The competition-stage analysis reports a **Random Forest AUC of 0.888**. Model output is interpreted as a decision-support ranking rather than an automatic installation decision.

## Portfolio-aligned representative figure

- Portfolio source: `Juna0926/Portfolio/assets/media/project-heated-detail.webp`
- The README displays this current Portfolio figure as its primary visual summary.

## Public file

- [`heated-pavement-analysis-public-excerpt.pdf`](heated-pavement-analysis-public-excerpt.pdf) — concise public-safe technical excerpt derived from the competition report.

## Supporting repository evidence

- `assets/figure-01-random-forest-auc.svg` — Random Forest ROC-AUC **0.888** and decision-support interpretation.
- `assets/figure-02-top-five-roads.svg` — highest-ranked candidate roads and the RF_probability values shown in the report.
- `assets/figure-03-expected-impact.svg` — expected impact and limitations reported by the project.

## Candidate-road validation

The original report additionally reviewed high-ranked roads using street-level context. The public repository summarizes that validation without redistributing third-party street imagery.

## Decision-support and limitation note

The ranking should be treated as a screening result. Engineering inspection, municipal feasibility, detailed road geometry, maintenance constraints, and field validation remain necessary before installation decisions.

Limitations preserved from the source material include:

- different update cycles across public datasets,
- potential coordinate / spatial preprocessing error,
- limited detailed road-width / environment data, and
- imbalance in road-type representation.

## Data note

Raw and intermediate public-data files are not redistributed because the analysis combines several external sources with distinct update cycles and usage conditions.
