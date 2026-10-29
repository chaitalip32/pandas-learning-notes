# Pandas Learning Notes

[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)

A structured, hands-on collection of notes, examples, and exercises
created while learning **Python Pandas**. This repository documents core
concepts through Jupyter Notebooks and practice datasets, with an
emphasis on understanding how to inspect, clean, transform, and analyse
tabular data.

> **Repository status:** Learning repository --- content is updated as
> new concepts and exercises are completed.

## Table of Contents

-   [About](#about)
-   [Learning Objectives](#learning-objectives)
-   [Topics Covered](#topics-covered)
-   [Repository Structure](#repository-structure)
-   [Tools and Technologies](#tools-and-technologies)
-   [Getting Started](#getting-started)
-   [How to Use the Notebooks](#how-to-use-the-notebooks)
-   [Practice Dataset](#practice-dataset)
-   [Contributing and Feedback](#contributing-and-feedback)
-   [Author](#author)

## About

Pandas is a Python library widely used for working with structured data.
I created this repository to keep my learning notes organised, practise
examples, and build a reusable reference for future data analysis and
data engineering work.

The notebooks combine explanations with code examples so that concepts
can be revisited and applied to datasets. The repository is intended for
beginners and other learners who want a practical introduction to
Pandas.

## Learning Objectives

-   Understand Pandas `Series` and `DataFrame` objects.
-   Load and inspect data from CSV files.
-   Select, create, insert, and remove DataFrame columns.
-   Apply arithmetic and logical operations.
-   Explore useful Pandas functions and methods.
-   Identify and handle missing data.
-   Practise data manipulation on tabular datasets.
-   Build a foundation for exploratory data analysis and data-focused
    projects.

## Topics Covered

  -----------------------------------------------------------------------
  Topic                               What I practise
  ----------------------------------- -----------------------------------
  Pandas data structures              Understanding `Series` and
                                      `DataFrame` concepts

  Arithmetic operations               Performing calculations across
                                      columns

  Logical operations                  Comparing values and evaluating
                                      conditions

  DataFrame column operations         Creating, inserting, and removing
                                      columns

  Pandas functions                    Exploring commonly used functions
                                      and methods

  CSV handling                        Working with tabular data stored in
                                      CSV files

  Missing data                        Identifying and handling absent
                                      values

  -----------------------------------------------------------------------

Topics and examples will expand as I continue learning.

## Repository Structure

``` text
## Repository Structure

```text
pandas-learning-notes/
│
├── README.md
├── Handling_Missing_Data_Replace_Interpolate_Notes.ipynb
├── Merge_and_Concat_DataFrames.ipynb
├── Pandas_GroupBy_Notes.ipynb
├── Pandas_Melt_Pivot_PivotTable_Notes.ipynb
├── handling_missing_data_notes.ipynb
├── pandas_csv_complete_notes.ipynb
├── pandas_data_structure_and_arithmetic_operations.ipynb
├── pandas_dataframe_insert_pop_del_notes.ipynb
├── pandas_functions.ipynb
└── sales.csv
```

### File Descriptions

| File | Description |
|---|---|
| `README.md` | Overview of the repository, learning objectives, and resources. |
| `Handling_Missing_Data_Replace_Interpolate_Notes.ipynb` | Notes and examples on handling missing data using replacement and interpolation techniques. |
| `Merge_and_Concat_DataFrames.ipynb` | Examples of merging and concatenating DataFrames. |
| `Pandas_GroupBy_Notes.ipynb` | Notes on grouping data and performing aggregate operations using `groupby()`. |
| `Pandas_Melt_Pivot_PivotTable_Notes.ipynb` | Examples of reshaping data using `melt()`, `pivot()`, and `pivot_table()`. |
| `handling_missing_data_notes.ipynb` | Notes on identifying, handling, and analyzing missing values. |
| `pandas_csv_complete_notes.ipynb` | Examples of importing, reading, and working with CSV files. |
| `pandas_data_structure_and_arithmetic_operations.ipynb` | Notes on Pandas data structures and arithmetic and logical operations. |
| `pandas_dataframe_insert_pop_del_notes.ipynb` | Examples of inserting, removing, and modifying DataFrame columns. |
| `pandas_functions.ipynb` | Notes and examples covering commonly used Pandas functions. |
| `sales.csv` | Sample sales dataset for practicing data manipulation and analysis. |
```

The structure above highlights the main files visible in the repository.
Filenames may change as the notes are reorganised.

## Tools and Technologies

-   **Python** --- programming language used for examples
-   **Pandas** --- data manipulation and analysis
-   **Jupyter Notebook** --- interactive notes, code, and outputs
-   **CSV** --- practice data format
-   **Git and GitHub** --- version control and repository hosting

## Getting Started

### Prerequisites

-   Python 3.8 or newer
-   `pip`, Python's package installer
-   Basic familiarity with running Python commands

### 1. Clone the repository

``` bash
git clone https://github.com/chaitalip32/pandas-learning-notes.git
cd pandas-learning-notes
```

### 2. Create and activate a virtual environment (recommended)

**Windows PowerShell**

``` powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux**

``` bash
python3 -m venv .venv
source .venv/bin/activate
```

If PowerShell blocks script activation because of your system's
execution policy, you can run the commands below without activating the
environment by using `.venv\Scripts\python.exe -m pip ...`, or use
Command Prompt activation with `.venv\Scripts\activate.bat`.

### 3. Install the packages

``` bash
python -m pip install --upgrade pip
python -m pip install pandas jupyter
```

### 4. Launch Jupyter Notebook

``` bash
jupyter notebook
```

Open a notebook (`.ipynb`) from the repository and run its cells in
order.

> **Note:** The current notebooks primarily use Pandas and Python's
> standard library. If a notebook later uses additional packages,
> install those packages as documented in that notebook.

## How to Use the Notebooks

1.  Start with the notebook whose topic you want to learn.
2.  Read the Markdown explanations before running the code.
3.  Run cells in order and inspect the outputs.
4.  Change example values to see how the results change.
5.  Try the same operations on `sales.csv`.
6.  Add your own examples and short explanations as you learn new
    concepts.

For the best results, use a local Python environment or another notebook
environment that supports Pandas. Some browser-based notebook
environments have restrictions on installing packages.

## Practice Dataset

The repository includes `sales.csv`, which can be used to practise
loading and exploring tabular data.

Example:

``` python
import pandas as pd

df = pd.read_csv("sales.csv")

print(df.head())
print(df.info())
print(df.describe(include="all"))
```

Try answering questions about the dataset, checking for missing values,
filtering rows, grouping records, and calculating summary statistics.

## Contributing and Feedback

This is primarily a personal learning repository. Suggestions,
corrections, and constructive feedback are welcome. If you spot an error
or have an idea for a useful beginner exercise, feel free to open an
issue or share feedback.

## Author

**Chaitali Pednekar**

-   GitHub: [@chaitalip32](https://github.com/chaitalip32)
-   Repository:
    [pandas-learning-notes](https://github.com/chaitalip32/pandas-learning-notes)

------------------------------------------------------------------------

*Learning in public, one Pandas concept at a time.*
