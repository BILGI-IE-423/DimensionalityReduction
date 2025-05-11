# DimensionalityReduction

# Lab Assignment: Dimensionality Reduction

## Objective
In this lab, you will learn how to reduce the dimensionality of high-dimensional datasets using **Principal Component Analysis (PCA)** and **t-distributed Stochastic Neighbor Embedding (t-SNE)**. You will apply these techniques to a dataset of music features and visualize the results to better understand their structure.

---

## Task 1: Load and Explore the Dataset

**Description**  
- Load the provided `music_data.mat` file.  
- Inspect its structure by printing the available keys.  
- Identify the matrix representing the features and the labels.

**Required Library**  
- `scipy.io`

---

## Task 2: Extract Features and Labels

**Description**  
- Extract the feature matrix (denoted as `X`) and the label array (denoted as `Y`) from the loaded data.  
- Examine the shapes of both arrays to ensure they are correctly formatted for analysis.

---

## Task 3: Normalize the Feature Matrix

**Description**  
- Normalize the feature matrix using **standardization**, so that each feature has zero mean and unit variance.  
- This step ensures that features with larger numeric ranges do not dominate the analysis.

**Required Library**  
- `sklearn.preprocessing.StandardScaler`

---

## Task 4: Apply Principal Component Analysis (PCA)

**Description**  
- Use PCA to reduce the dimensionality of the feature matrix to two components.  
- Visualize the transformed data in a 2D scatter plot where each point is colored according to its label.

**Required Libraries**  
- `sklearn.decomposition.PCA`  
- `matplotlib.pyplot`

---

## Task 5: Apply t-SNE for Dimensionality Reduction

**Description**  
- Apply **t-distributed Stochastic Neighbor Embedding (t-SNE)** to the same normalized feature matrix to reduce it to two dimensions.  
- Generate a 2D visualization where the points are colored by their class labels.  
- Observe the differences in how t-SNE and PCA represent the data.

**Required Library**  
- `sklearn.manifold.TSNE`

---

## Task 6: Compare and Interpret PCA and t-SNE Visualizations

**Description**  
- Analyze the visualizations from both PCA and t-SNE.  
- Consider the following:
  - Which method produces more distinguishable clusters?
  - Which technique better preserves the local structure of the data?
  - How does the choice of dimensionality reduction method affect interpretability?
