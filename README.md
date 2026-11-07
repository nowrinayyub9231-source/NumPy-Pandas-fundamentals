# NumPy & Pandas Fundamentals: Assignment 10

A hands-on Jupyter notebook covering the core building blocks of data analysis in Python: **NumPy arrays**, **Pandas Series**, and **Pandas DataFrames**. Each section uses a small, realistic dataset (weekly temperatures, student marks, and retail transactions) to practise creating, inspecting, slicing, filtering, and modifying data.

---

## Table of Contents

- [Overview](#overview)
- [What's Covered](#whats-covered)
- [Datasets Used](#datasets-used)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)
- [Key Takeaways](#key-takeaways)
- [Author](#author)

---

## Overview

This assignment builds practical fluency with the two libraries at the heart of the Python data stack. The notebook walks through each task step by step, with short comments explaining what each cell does.

## What's Covered

### 1. NumPy Array Operations

| Topic | Details |
|---|---|
| **1D arrays** | Creating an array of daily temperatures for one week |
| **Inspection** | Using `.shape`, `.dtype`, and `.size` |
| **Array operations** | Celsius → Fahrenheit conversion using vectorised arithmetic; `max`, `min`, and `mean` |
| **Slicing & indexing** | First three days, weekend (last two days), and middle three days |
| **2D arrays** | Building a two-week temperature matrix |
| **2D slicing** | Extracting each week and each weekend from the matrix |

### 2. Pandas Series

| Topic | Details |
|---|---|
| **Creation** | A Series of student marks with a custom index (`Rank 1` to `Rank 5`) |
| **Indexing** | Position-based (`iloc`) and label-based (`loc`) access |
| **Boolean masking** | Filtering ranks where marks are above 90 |
| **Manipulation** | Updating a value, dropping an entry, and deriving CGPA (marks ÷ 10) |

### 3. Pandas DataFrame

| Topic | Details |
|---|---|
| **Creation** | Building a transactions DataFrame from a dictionary |
| **Exploration** | `head()`, `tail()`, `shape`, `columns`, `dtypes` |
| **Selection** | Selecting columns and slicing with `loc` |
| **Filtering** | Combining conditions (e.g. Region = North **and** Amount > 200) |
| **Summaries** | `value_counts()`, `unique()`, and `groupby()` with mean |
| **Manipulation** | Updating a value, adding a `Discount` column (10% of Amount), dropping a row, dropping a column |

## Datasets Used

All data is defined inside the notebook, so there are **no external files to download**.

- **Temperatures:** 7 daily readings (week 1) plus a second week to form a 2 × 7 array
- **Marks:** 5 student scores indexed by rank
- **Transactions:** 10 records with `Transaction_ID`, `Product_Category`, `Region`, and `Amount`

## Tech Stack

- **Python** 3.8+
- **NumPy**
- **Pandas**
- **Jupyter Notebook**

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

### 2. Install dependencies

```bash
pip install numpy pandas notebook
```

### 3. Launch the notebook

```bash
jupyter notebook Assignment_10.ipynb
```

Then run the cells from top to bottom using **Kernel → Restart & Run All**.

## Repository Structure

```
.
├── Assignment_10.ipynb   # Main notebook with all exercises
└── README.md             # Project documentation
```

## Key Takeaways

- NumPy's vectorised operations make bulk calculations (like unit conversion) fast and concise, with no loops needed.
- `iloc` selects by **position**, while `loc` selects by **label**. Knowing which to use avoids subtle indexing bugs.
- Boolean masks, including combined conditions with `&`, are the foundation of filtering data in Pandas.
- `groupby()` and `value_counts()` give quick summaries of categorical data.
- Updating values with `.loc[condition, column]` is safer than chained indexing.

## Author

**Nowrin**
Microbiology graduate transitioning into data analytics

- LinkedIn: https://www.linkedin.com/in/nowryub

- GitHub: https://github.com/nowrinayyub9231-source
