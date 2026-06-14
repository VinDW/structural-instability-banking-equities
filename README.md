# Structural Instability in Big Five South African Banking Equities

This repository contains the Python notebook used for Paper 1 of the banking-equity volatility project.

## Project focus

The notebook analyses structural instability and volatility shifts in the Big Five South African banking equities:

- Standard Bank
- FirstRand
- Absa
- Nedbank
- Capitec

The analysis uses daily closing prices from the IRESS Research Domain dataset. Because the IRESS data are proprietary, the raw Excel file is not included in this repository.

## Repository structure

```text
.
├── data/
│   └── README.md
├── figures/
│   └── .gitkeep
├── notebooks/
│   └── 01_structural_instability_break_detection.ipynb
├── outputs/
│   └── .gitkeep
├── .gitignore
├── README.md
└── requirements.txt
```

## Methods included

The notebook reproduces the main empirical workflow:

1. Data loading and cleaning
2. Daily log-return construction
3. Absolute-return and squared-return transformations
4. Descriptive statistics and Jarque-Bera normality testing
5. Multiple structural-break detection using BIC selection
6. ICSS variance-break detection
7. Adjacent-regime validation using distributional and variance tests
8. Monthly break clustering
9. Composite Structural Instability Score (CSIS)
10. Export of tables, figures and final workbook

## How to run

1. Clone or download the repository.
2. Place your IRESS Excel file in the `data/` folder.
3. Rename the file as:

```text
IRESS_DATASET.xlsx
```

4. Install the required packages:

```bash
pip install -r requirements.txt
```

5. Open and run:

```text
notebooks/01_structural_instability_break_detection.ipynb
```

Generated tables will be saved in the `outputs/` folder and figures will be saved in the `figures/` folder.

## Data note

The IRESS Research Domain dataset is not shared in this repository. Users must supply their own authorised data file.

## Author

Mojaesi Vincent Kometsi  
School of Agriculture, Engineering and Science, Discipline of Statistics  
University of KwaZulu-Natal, Durban, South Africa
