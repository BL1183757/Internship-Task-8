# Internship-Task-8

## Customer Segmentation with K-Means Clustering

This project demonstrates **unsupervised machine learning** techniques to segment customers based on their profile and spending behavior. Using the **K-Means clustering algorithm**, we group customers with similar characteristics to aid in targeted marketing strategies.

## Project Overview

- **Dataset**: Contains `CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, and `Spending Score (1–100)`.
- **Goal**: Identify distinct groups in customer data based on age, annual income, and spending score.
- **Algorithm Used**: [K-Means Clustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

## 🗂 Dataset Description

| Column                  | Description |
|-------------------------|-------------|
| **CustomerID**          | Unique identifier for customers |
| **Genre**               | Gender of the customer |
| **Age**                 | Age of the customer |
| **Annual Income (k$)**  | Annual income in thousand dollars |
| **Spending Score (1-100)** | Spending behavior score assigned by the mall |

## ⚙️ Installation

## To install required dependencies, run:
    pip install pandas numpy matplotlib seaborn scikit-learn


## Steps Performed

1. **Load Data**
   - Imported the dataset into a Pandas DataFrame.
   - Inspected structure and statistics.

2. **Data Preprocessing**
   - Selected relevant features (`Age`, `Annual Income (k$)`, `Spending Score (1-100)`).
   - Scaled numerical features using `StandardScaler`.
   - Encoded categorical variables (if any) using `OrdinalEncoder`.

3. **Clustering**
   - Applied **K-Means** clustering for `n_clusters=5`.
   - Evaluated cluster performance with **Silhouette Score**.

4. **Dimensionality Reduction (PCA)**
   - Used **PCA** to reduce features to 2D space for visualization.

5. **Visualization**
   - Plotted clusters using Matplotlib & Seaborn.
   - Displayed cluster centers and separation.

## Results

- Developed **5 customer segments**, each showing unique combinations of income and spending behavior.
- Identified distinct high-income/high-spending clusters and low-income/low-spending clusters.

## How to Run

### Clone this repository
    git clone https://github.com/BL1183757/Internship-Task-8.git
    cd Internship-Task-8.git
### Install dependencies
    pip install -r requirements.txt
### Run the notebook:
    jupyter notebook Task-8.ipynb

4. Run all cells to reproduce the preprocessing, clustering, and visualization.

## Example Segments

| Cluster | Characteristics |
|---------|-----------------|
| 0       | Middle income, average spending |
| 1       | Older age, moderate spending |
| 2       | High income, high spending |
| 3       | Younger customers, high spending |
| 4       | Low income, low spending |

## License

This project is for **educational purposes** and free to use.

---

**Author**: *Bhavay Khandelwal*  
**Date**: 15th August 2025
