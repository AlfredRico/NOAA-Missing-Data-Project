# NOAA Lightning Strike Missing Data Analysis

---

## Overview

This project analyzes lightning strike data across geographic locations with a focus on handling missing data and validating dataset consistency through merging and spatial analysis.

---

## Key Insights

* A large portion of missing zip/state data occurs because many lightning strikes happen outside U.S. mappable regions (over water or in other countries), where U.S. geographic identifiers do not exist.
* The missing values are not a primary data quality issue, rather a data scope mismatch
* Most of the missing data is expected and acceptable or can be addressed via the database owners  

---

## Reproducibility

This project uses **UV** for fast, deterministic environment management.

### 🔧 Prerequisites

Install UV (official guide):  
https://docs.astral.sh/uv/getting-started/

---

### ▶️ Run Locally (Step-by-Step)

```bash
# 1. Clone the repository
git clone https://github.com/AlfredRico/NOAA-Missing-Data-Project.git
cd NOAA-Missing-Data-Project

# 2. Sync environment (installs Python + dependencies)
uv sync

# 3. Launch Jupyter Lab
uv run jupyter lab
```

---

### 📂 Open the Project

Once Jupyter Lab opens in your browser:

1. Navigate to the project root directory  
2. Open the notebook:

   ```
   noaa_missing_data_analysis.ipynb
   ```

3. Run all cells from top to bottom  

---

### 🧠 Notes

- The environment is fully defined by:
  - `pyproject.toml`
  - `uv.lock`
- No manual package installation is required  
- Results are fully reproducible across systems  

---

## Project Structure

```
NOAA-Missing-Data-Project/
├── data/eda_missing_data_dataset2.csv   # sample dataset (tracked)
├── noaa_missing_data_analysis.ipynb
├── pyproject.toml
├── uv.lock
└── README.md
```

---

## Data Source

This notebook uses two .csv files: 

eda_missing_data_dataset1.csv 

eda_missing_data_dataset2.csv

Both files come from the bigquery-public-data.noaa_lightning.lightning_strikes public data table.

> Note: Only a sample dataset is included for reproducibility.  
> The full dataset can be obtained from the source above.

---

## Ecosystem

* Portfolio webpage → Project hub and navigation: https://alfredrico.github.io/  
* GitHub → Project repositories featuring UV management for reproducibility: https://github.com/AlfredRico  