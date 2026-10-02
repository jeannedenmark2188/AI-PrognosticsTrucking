# Cross-Manufacturer AI Prognostics for Heavy-Duty Trucking

Doctoral dissertation research on AI-based telematics and prognostics for heavy-duty trucking fleets. The project applies cross-manufacturer transfer learning, privacy-preserving federated learning, and stakeholder interpretability methods to predictive maintenance, and links vehicle health signals to safety outcomes using public safety data.

- **Author:** Jeanne Denmark
- **Advisor:** Dr. Aledhari
- **Target venue:** PHM Society Annual Conference Doctoral Symposium

## Research overview

The dissertation is organized around four studies:

1. **Cross-manufacturer transfer learning** for predictive maintenance across different truck manufacturers
2. **Privacy-preserving federated learning** across fleets
3. **Stakeholder interpretation** of AI model outputs
4. **Health-to-safety linkage**, connecting vehicle health data to safety outcomes using public FMCSA and NHTSA data

## Repository structure

```
.
├── data/              # Dataset documentation and public data (see Data below)
├── src/               # Source code — preprocessing, modeling, evaluation
├── notebooks/         # Exploratory analysis and experiment notebooks
├── results/           # Current model outputs, metrics, evaluation artifacts
├── figures/           # Current charts and visualizations used in the manuscript
├── manuscript/        # Current draft(s) of the dissertation / paper manuscript
├── references/        # Bibliography and reference material
└── README.md
```

Only current working versions are kept in each folder — superseded drafts and old result runs are not retained in the repo.

## Data

This project uses three datasets:

| Dataset | Access | Notes |
|---|---|---|
| SCANIA Component X | Public | Benchmark dataset for predictive maintenance |
| Volvo Discovery Challenge (ECML-PKDD 2024) | Public | Second public benchmark, added so core findings don't depend solely on private data |
| PACCAR fleet telematics | Private / restricted | See **PACCAR data policy** below |

Public datasets, or links/instructions for obtaining them, live under `data/`.

### PACCAR data policy

Use of PACCAR fleet telematics data in this research is governed by a signed data use authorization with PACCAR. Under that authorization:

- **No customer data** of any kind (names, accounts, contact or billing information, or anything identifying a specific customer or fleet owner) is used in this research.
- **Vehicles are referenced only by the last six (6) digits of the VIN.** Full VINs are never recorded, stored, or committed to this repository.
- **No PACCAR telematics data — raw or processed — is uploaded to this repository** unless and until it is confirmed that the data use authorization permits storing it on GitHub, even in a private repo. Until then, the `data/paccar/` folder contains only a description of the data (source, fields, and how to obtain access) rather than the data itself.
- The same restriction applies to any data obtained through the PACCAR marketing-team benchmarking collaboration.
- Open/public competitor data may be included in this repository as usual, with its source and license documented in `data/`.

## Collaboration workflow

- Updates are tracked via commits and pushes, with a summary of what changed noted in the commit message or in this README.
- A short email is sent to the advisor when an update is ready for review, rather than attaching files directly.

## Contact

Questions about this repository or the research can be directed to Jeanne Denmark.
