# Iris Dataset Analysis

## Project Overview

This project analyzes the Iris dataset using Python, Pandas, and Jupyter Notebook. The goal is to explore the data, check for missing and duplicate values, calculate basic statistics, and compare different flower species.

## Tools Used

- **Python:** Programming language used for the analysis.
- **uv:** Manages the project environment and dependencies.
- **Pandas:** Used to read, clean, and analyze the dataset.
- **Jupyter Notebook:** Used to write and run the analysis code.

## Setup Instructions

1. Install uv if it is not already installed:
   ```bash
   curl -LsSf https://astral.sh/uv/install.sh | sh
   ```
2. Create the project and navigate to its folder:
   ```bash
   uv init iris-analysis
   cd iris-analysis
   ```
3. Create and activate a virtual environment:
   ```bash
   uv venv
   source .venv/bin/activate
   ```
4. Install the required packages:
   ```bash
   uv add pandas notebook
   ```
5. Download the dataset:
   ```bash
   mkdir -p data
   curl -o data/iris.csv https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv
   ```
6. Start Jupyter Notebook:
   ```bash
   uv run jupyter notebook
   ```
7. Open `iris_analysis.ipynb` and run all cells.

## Summary of Findings

- The dataset contains 150 rows and 5 columns.
- No missing values were found.
- One duplicate row was identified.
- The dataset contains three species: Setosa, Versicolor, and Virginica, with 50 flowers per species.
- The average sepal length is approximately 5.84 cm.
- The maximum petal length is 6.9 cm.
- The minimum sepal width is 2.0 cm.
- 61 flowers have a sepal length greater than 6 cm.
- 52 flowers have a petal width greater than 1.5 cm.
- Virginica has the highest average petal length, while Setosa has the lowest.

## Project Structure

```
iris-analysis/
├── pyproject.toml
├── uv.lock
├── iris_analysis.ipynb
├── README.md
├── data/
│   └── iris.csv
└── output/
    ├── species_summary.csv
    └── filtered_iris.csv
```

## Conclusion

This project provides practice in loading CSV files, exploring datasets, calculating statistics, filtering rows, grouping data, and exporting results using Pandas.
