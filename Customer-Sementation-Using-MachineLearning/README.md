# Customer Segmentation using Machine Learning

This project segments wholesale distribution customers into distinct groups based on their annual spending across product categories, so a business can target marketing and account management differently per group — and specifically identifies which segment is **highest-value**.

**Techniques used:** data cleaning, log-transform + standardization to correct for skew, PCA (for 2D visualization), K-Means clustering with the number of clusters chosen via the elbow method and silhouette analysis, cluster evaluation (silhouette score, Calinski-Harabasz index), and cluster profiling to turn the math into a business recommendation.

**Dataset:** [Wholesale customers dataset](https://archive.ics.uci.edu/dataset/292/wholesale+customers) (included as `wholesale_customers.csv`) — 440 customers of a wholesale distributor, with annual spend on Fresh, Milk, Grocery, Frozen, Detergents_Paper, and Delicassen products.

## Getting Started

### Prerequisites

Python 3.9+ and the packages listed in `requirements.txt`:

```
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

### Installation

```bash
pip install -r requirements.txt
```

### Usage

1. Clone or download this repository.
2. From the project directory, launch Jupyter:

   ```bash
   jupyter notebook
   ```

3. Open `Customer Segmentation using Machine Learning.ipynb`.
4. Run all cells (Kernel → Restart & Run All). The notebook is self-contained — it loads `wholesale_customers.csv` from the same folder.

## What the notebook produces

- EDA plots (boxplots, correlation heatmap) showing spend distribution and category relationships
- An elbow-method + silhouette-score comparison used to choose the number of clusters
- A trained K-Means model with quantitative evaluation (silhouette score, Calinski-Harabasz index)
- A PCA scatter plot of the resulting customer segments
- A cluster profile table/heatmap showing average spend per category, per segment
- A written business-insights section identifying the high-value customer segment and a recommended strategy per segment

## Author

Rituraj Das — [GitHub](https://github.com/rituraj124) · [LinkedIn](https://www.linkedin.com/in/rituraj-das-11439b356/)

