# 📊 INF/01 Q1 Journal Metrics

## 📝 Description
This repository contains a curated dataset of **Q1 (Class A)** academic journals within the **INF/01 (Computer Science)** sector. The data is derived from official bibliometric calibrations and filtered to include only high-impact publications recognized for research excellence.

## 🚀 Key Features
- **Q1 Focus**: Exclusively lists journals classified as "Classe A" (Top Tier).
- **Structured Data**: Cleaned CSV dataset ready for statistical analysis and integration.
- **Academic Transparency**: Fully documented selection and filtering methodology.

## 📂 Repository Structure
- `data/journals.csv`: The primary dataset containing filtered journals and their respective metrics.
- `docs/methodology.md`: Detailed documentation of inclusion criteria and data processing steps.

## 🛠 Usage
The `journals.csv` file is compatible with Excel, Python (Pandas), or R:
```python
import pandas as pd
df = pd.read_csv('data/journals.csv')
# Display the top-ranked journals in the dataset
print(df.head())

```

## 📊 Dataset Schema

The CSV follows this structure:
| Column | Description |
| :--- | :--- |
| **Rivista** | Official Journal Name |
| **A** | Excellence Indicator (Class A / Top 10%) |
| **B, C, D, E** | Distribution across lower impact percentiles |

---

✨ *Advancing transparency in scientific research evaluation.* ✨

