# NanoDrop Chromatography Fitting and Purity Analysis

This repository contains the R code and input data used to perform chromatographic trace fitting and purity estimation in our paper:
"A facile and reproducible method for the purification of peptide- and protein-functionalized DNA nanostructures "

---

## Fitting motivation

We model NanoDrop-based elution profiles using a **sum of two log-normal probability density functions** to:

- Deconvolve overlapping peaks
- Calculate **resolution (Rs)** between peaks
- Estimate **fractional purity** across elution volumes

---

## Repository Contents

| File | Description |
|------|-------------|
| `NanoDrop_Nanostructures.xlsx` | Input data file  Elution Volume + Samples |
| `Fitted_NanoDrop_Summary.csv` | Output data file  Elution Volume + Samples + Purities|
| `Automated_fitting_purity_resolution_script.rmd` | Main R script for fitting, purity calculation, and plotting |
| `README.md` | |

---

## Key Outputs

Running the script produces:

- **Purity plots** with fitted peak curves, shaded AUCs, purity labels, and parameter annotations
- **Mean trace** plot with standard deviation error bars
- A combined output table (`final_table`) containing:
  - Elution volumes
  - Raw traces
  - Per-sample purities
  - Mean purity per fraction
  - Standard deviation of purity

No plots are included in the repo; instead, they repoduceable with the included excel file

---
## AI Disclosure:
The code was written with the assistance of LLMs
## License

This project is licensed under the [MIT License](LICENSE) — you are free to use, share, and adapt the code with attribution.

## 🔧 Clone this repository:
   ```bash
   git clone https://github.com/yourusername/NanoDropPurityFit.git



