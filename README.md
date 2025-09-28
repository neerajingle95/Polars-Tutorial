# Polars Tutorial

This repository contains code and notebooks from the Polars tutorial series based on this video lecture:  
👉 [Polars Tutorial Video](https://www.youtube.com/watch?v=8GoBlwgbirE&t=975s)

The dataset used in the tutorial is a sample **transactions Parquet file**, available here:  
[transactions.parquet](https://storage.googleapis.com/rapidsai/polars-demo/transactions.parquet)

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/neerajingle95/Polars-Tutorial.git
cd Polars-Tutorial
```

### 2. Setup environment
Using venv or conda is recommended. For example, with venv:

```bash
python3 -m venv venv
source venv/bin/activate
```

You would need to install the following libraries:
polars
pyarrow
hvplot[polars]
jupyterlab

### 3. Download dataset (if not already present)
The tutorial expects a Parquet file named transactions.parquet. You can download it manually using the link given at the top.

## 🧪 Using the Tutorial
1. Launch JupyterLab / Jupyter Notebook:

```bash
jupyter lab
```

2. Open the notebook(s) in the notebooks/ folder and run through the examples.

3. Explore Polars features such as:
- Reading Parquet / CSV files
- Filtering, grouping, aggregations
- Lazy execution
- Plotting

## 💡 Key Learning Outcomes
By working through this tutorial, you will:
- Understand the Polars DataFrame API and how it compares to pandas
- Learn to leverage Polars' lazy evaluation for performance
- Practice common data transformations and aggregations
- Gain experience working with Parquet files and real-world tabular data
- Generate interactive visualizations using hvplot with Polars

## 🛠️ Tips & Troubleshooting
If you see ModuleUpgradeRequiredError: hvplot>=0.9.1 is required for .plot, ensure you installed hvplot in the same environment your notebook is running in, e.g.:

```bash
pip install --upgrade hvplot
pip install polars[hvplot]
```

If you face ModuleNotFoundError: pa.Table requires 'pyarrow' module to be installed, double check:

```bash
pip install pyarrow
```
and restart your notebook kernel.
