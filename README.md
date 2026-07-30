# PySpark Superstore Analysis

A PySpark project for exploring and analyzing the classic Superstore sales dataset - built while applying the fundamentals of Spark and PySpark learned from an introductory Course.

## 📌 Project Overview

This project uses PySpark's DataFrame API to load, clean, and analyze the Superstore dataset. The goal is to practice core Spark concepts (SparkSession, DataFrames, transformations, aggregations) on a real-world tabular dataset, and produce processed outputs that can be visualized separately.

## 🗂️ Project Structure

```
PYSPARK_PROJECT/
├── processed_data/        # Output of analysis.ipynb - aggregated/cleaned data used for visualizations
├── venv/                  # Python virtual environment (not tracked in git)
├── .gitignore
├── analysis.ipynb         # Main notebook: data loading, cleaning, EDA, and aggregations
├── visualizations.ipynb   # Notebook for charts based on processed_data (WIP)
├── requirements.txt       # Project dependencies
├── superstore_data.csv    # Source dataset
└── README.md
```

## ⚙️ Tech Stack

- **PySpark** - distributed data processing and analysis
- **Jupyter Notebook** - interactive development
- **VS Code** - development environment
- Python virtual environment for dependency management

## 🚀 Getting Started

### Prerequisites
- Python 3.x
- Java (required for Spark)
- pip

### Setup

1. Clone the repository
   ```bash
   git clone https://github.com/Het25Dave/superstore_analysis_using_pyspark
   cd PYSPARK_PROJECT
   ```

2. Create and activate a virtual environment
   ```bash
   python -m venv venv
   # Windows
   venv\Scripts\activate
   # macOS/Linux
   source venv/bin/activate
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Open `analysis.ipynb` in VS Code or Jupyter and run the cells.

## 🔍 What `analysis.ipynb` Does

1. **Initialize Spark** - creates a `SparkSession` as the entry point to Spark.
2. **Load Data** - reads `superstore_data.csv` into a Spark DataFrame.
3. **Data Cleaning**
   - Renames columns for consistency (e.g., removing spaces, standardizing casing).
   - Corrects column data types (e.g., dates, numeric fields) that weren't inferred correctly on load.
4. **Exploratory Data Analysis (EDA)** - inspects schema, checks summary statistics, and reviews the dataset's structure.
5. **Aggregations** - groups and summarizes the data (e.g., by region, category, or other dimensions) using PySpark's DataFrame API.
6. **Export Results** - saves the processed/aggregated outputs to the `processed_data/` folder, to be used as input for the visualizations notebook.

## 📊 Visualizations

`visualizations.ipynb` is a **work in progress**. It will read from `processed_data/` and generate charts based on the aggregated results from the analysis notebook.

## 📈 Dataset

The project uses the **Superstore dataset**, a commonly used retail dataset containing sales, profit, customer, and order information - often used for practicing data analysis and BI concepts.

## 🎓 Background

This project was built as a hands-on follow-up to a beginner-level PySpark course, applying core concepts like SparkSessions, DataFrame transformations, and aggregations to a real dataset.

## 📝 Notes

- This is a learning project focused on fundamentals - expect basic, straightforward transformations rather than advanced Spark features.
- `visualizations.ipynb` will be updated as charts are added.
