# Public Project Outputs

## Source artifact reviewed

- `2025 광진구 빅데이터 분석 공모전 - 광진구 열선 설치 우선 도로 예측 ML 모델 생성` analysis report.

## Public file

- [`heated-pavement-analysis-public-excerpt.pdf`](heated-pavement-analysis-public-excerpt.pdf) - concise public-safe technical excerpt derived from the competition report.

## Public-safe evidence included

- `assets/figure-01-random-forest-auc.svg` - Random Forest ROC-AUC 0.888 and decision-support interpretation.
- `assets/figure-02-top-five-roads.svg` - five highest-ranked roads and the RF_probability values shown in the report.
- `assets/figure-03-expected-impact.svg` - expected impact and limitations reported by the project.

## Candidate-road validation

The original report additionally reviewed the top-ranked roads using street-level context. The public repository summarizes that validation without redistributing third-party street imagery.

## Limitations preserved from the report

- Different update cycles across public datasets
- Potential coordinate / spatial preprocessing error
- Limited detailed road-width / environment data
- Imbalance in road-type representation

## Data note

Raw and intermediate public-data files are not redistributed because the analysis combines several external sources with distinct update cycles and usage conditions.
