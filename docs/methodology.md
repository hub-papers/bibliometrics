# 📚 Methodology

## 🎯 Project Objective
This repository aims to maintain a curated list of academic journals and compute specific performance metrics. 
The primary goal is to provide a standardized framework for evaluating journal impact and quality within the INF/01 scientific sector.

## 🛠 Data Processing Workflow

The data pipeline consists of the following stages:

1.  **Data Extraction 📥**
    * Raw data is retrieved from official institutional documents (e.g., University of Cagliari bibliometric reports).
    * Text cleaning is performed to resolve formatting inconsistencies and multi-line journal titles.

2.  **Filtering & Selection 🔍**
    * Strict inclusion criteria are applied. Journals classified as `"NO CLASSE A"` are systematically excluded to focus the analysis on high-tier publications.

3.  **Metrics Computation 🧮**
    * Journals are categorized into merit classes (A, B, C, D, E).
    * Distribution metrics are calculated based on percentile thresholds (e.g., Top 10%, 10-35%).
    * Rankings are generated according to the latest bibliometric calibration (Ref: 24/06/2024).

4.  **Output Generation 📄**
    * Refined datasets are exported in `.csv` format to ensure interoperability with statistical analysis tools (R, Python, Excel).

## 📊 Data Structure
Each entry in the final dataset includes:
- 📖 **Journal**: Full official title.
- ⭐ **Class A**: Excellence indicators (Top 10%).
- 📈 **Classes B-E**: Tiered impact distribution.

## ⚖️ Transparency Statement
All metrics are derived from the most recent available calibration data. This project is open-source to ensure reproducibility and community-driven refinement of the parsing logic. 💻

---
✨ *Maintained for academic transparency and research evaluation.* ✨