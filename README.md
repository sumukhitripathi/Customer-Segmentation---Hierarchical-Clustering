# Customer Segmentation - Hierarchical Clustering

This project applies hierarchical clustering to an online retail dataset and generates a dendrogram visualization. It is a compact machine learning mini project for exploring customer or transaction grouping from numeric retail features.

## Project Overview

The script:

1. Loads `online_retail.csv`.
2. Selects numeric columns from the dataset.
3. Drops missing values.
4. Applies Ward hierarchical clustering using SciPy.
5. Saves the dendrogram as `dendrogram.png`.

## Dataset

The included dataset is `online_retail.csv`, with columns such as:

- `InvoiceNo`
- `StockCode`
- `Description`
- `Quantity`
- `InvoiceDate`
- `UnitPrice`
- `CustomerID`
- `Country`

Only numeric columns are used for clustering.

## Requirements

Install the required Python libraries:

```bash
pip install pandas matplotlib scipy
```

## How to Run

From the project directory, run:

```bash
python main.py
```

After execution, the project will generate:

```text
dendrogram.png
```

## Project Structure

```text
.
+-- main.py
+-- online_retail.csv
+-- README.md
```

## Output

The generated dendrogram shows the hierarchical relationship between data points based on the selected numeric features. It can be used to visually inspect possible customer or transaction segments.

## Notes

- The clustering uses the Ward linkage method.
- The current script clusters rows directly from the numeric dataset.
- For larger datasets, hierarchical clustering can become computationally expensive.