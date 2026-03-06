<div align="center">

# 🌧️ India Rainfall Data Visualization (1901–2015)

### 115 Years of Indian Monsoon Patterns Across Three Chart Types

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge)](https://matplotlib.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge)](LICENSE)

<br/>

> A multi-chart analysis of India's historical area-weighted rainfall data from 1901 to 2015, exploring annual trends, per-month patterns, and seasonal distribution through three distinct visualization strategies.

</div>

---

## Overview

This project uses a single well-structured dataset — India's area-weighted annual rainfall — to demonstrate how different chart types reveal different aspects of the same data. The Jun–Sep monsoon season's visual dominance in the bubble plot immediately communicates why it accounts for over 70% of India's annual rainfall.

| Dimension | Value |
|-----------|-------|
| Dataset | `rainfall_area-wt_India_1901-2015.csv` |
| Timespan | 115 years (1901–2015) |
| Columns | 12 monthly + 4 seasonal + annual totals |
| Visualizations | 3 chart types (line, scatter × 12, seasonal overlay) |

---

## Visualizations

### Chart 1 — Annual Rainfall Trend (Line Chart)
Long-term annual variation from 1901–2015 with marked data points, showing inter-annual variability and the absence of a strong trend in total annual rainfall.

### Chart 2 — Monthly Patterns (12 Scatter Plots)
A `for` loop generates one scatter plot per month (JAN–DEC). The **viridis colormap** is applied using the year index as the color variable, making decade-level changes visually apparent. The bubble size equals the rainfall value — visually heavier for wet months.

### Chart 3 — Seasonal Overlay (Bubble Scatter)
Four overlaid series (Jan-Feb, Mar-May, Jun-Sep, Oct-Dec) in distinct colors with bubble size proportional to rainfall. The **Jun–Sep monsoon season dominates** visually, confirming it as India's primary rainfall driver.

---

## Tech Stack

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading and column selection |
| `numpy` | Array range generation for colormap |
| `matplotlib` | All three chart types (line, scatter, overlay) |

---

## Key Observation

The Jun–Sep season consistently produces bubbles significantly larger than all other seasons combined, providing immediate visual confirmation that India's climate is **monsoon-dominated** — a pattern stable across all 115 years in the dataset.

---

## How to Run

```bash
pip install pandas numpy matplotlib jupyter
jupyter notebook "Rainfall(1901-2015) (1).ipynb"
```

> **Note:** Place `rainfall_area-wt_India_1901-2015.csv` in the same directory before running.
