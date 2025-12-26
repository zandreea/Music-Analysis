# 💻 Setting up

### 1. 🛠️ Set up project

- `git clone` or `mkdir` a project folder.
- `cd` to project directory.
- Make sure you have Python3 installed: `python --version`.

### 2. 🧪 Set up virtual environment

> A virtual env creates an isolated Python environment for a project, keeping its dependencies separate from other projects and the system Python. 

```bash
python3 -m venv .venv # Create
source .venv/bin/activate # Activate
```

### 3. Install dependencies

```bash
pip install --upgrade pip
pip install jupyter pandas numpy matplotlib seaborn scikit-learn ipykernel
```

### 4. Set up VS Code

- Install the **Python** and **Jupyter** extensions in VS Code.
- Open current directory in vs code: `code .`.
- 

# 🧹 Cleaning Up

To remove the virtual environment:

```bash
deactivate
rm -rf venv
```

# Tools & Libraries

### 🪐 jupyter – Interactive Coding Environment

Lets you write and run code in "cells", making it easy to test, visualize, document code in markdown and have the results too.

### 🐼 pandas – Data Handling & Analysis

Provides powerful data structures (DataFrame, Series) for working with structured (tabular) data.

Makes it easy to read from CSVs, clean, filter, group, and manipulate data efficiently.

Example use case: Loading a CSV of sales data, filtering by month, grouping by product.

```python
import pandas as pd
df = pd.read_csv('data.csv')
df.groupby('category').sum()
```

### 🔢 numpy – Numerical Computation & Arrays

Numerical computing with fast array/matrix operations.

Underpins many other libraries (like pandas and scikit-learn); enables fast operations on large datasets.

Example use case: Vector math, random number generation, reshaping arrays.

```python
import numpy as np
arr = np.array([1, 2, 3])
arr * 2  
# array([2, 4, 6])
```

### 📊 matplotlib – Basic Data Visualization

Creates static, animated, or interactive 2D plots and charts.

It's the standard for plotting in Python; gives fine control over plot appearance.

Example use case: Line charts, bar plots, scatter plots.

```python
import matplotlib.pyplot as plt
plt.plot([1, 2, 3], [4, 5, 6])
plt.show()
```

### 📈 seaborn – Statistical Visualization

Built on top of matplotlib for prettier, higher-level statistical plots.

Easier syntax and better styling than plain matplotlib; adds things like heatmaps, violin plots, correlation plots.

Example use case: Visualizing distributions, categorical data, or heatmaps of correlations.

```python
import seaborn as sns
sns.boxplot(x='species', y='sepal_length', data=df)
```

### 🤖 scikit-learn – Machine Learning

Provides ML algorithms and tools: clustering, classification, regression, dimensionality reduction, model evaluation.

Easy-to-use and consistent API for many algorithms (e.g., KMeans, RandomForest, PCA).

Example use case: Train a model to classify spam vs ham, or cluster customers.

```python
from sklearn.cluster import KMeans
kmeans = KMeans(n_clusters=3).fit(data)
```
