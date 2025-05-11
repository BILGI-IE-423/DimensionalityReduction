# Lab Assignment: Dimensionality Reduction

## Objective
Explore how dimensionality reduction techniques can help in understanding high-dimensional datasets. You will work with PCA and t-SNE using both 2 and 3 components, and compare their effectiveness.

---

## Task 1: Load and Inspect the Data

**Description**  
- Load the dataset `music_data.mat`.
- Inspect the keys and understand what each entry represents.

**Required Library**  
- `scipy.io`

---

## Task 2: Extract Features and Labels

**Description**  
- Extract the feature matrix (`X`) and label array (`Y`) from the dataset.
- Confirm their shapes.

---

## Task 3: Normalize the Data

**Description**  
- Use standardization (zero mean, unit variance) to normalize `X`.

**Required Library**  
- `sklearn.preprocessing.StandardScaler`

---

## Task 4: Apply PCA and t-SNE with 2 Components

**Description**  
- Apply PCA to reduce the data to 2 components.
- Apply t-SNE to reduce the data to 2 components.
- Create 2D scatter plots for each method.
- Label each point using the values in `Y`.

**Required Libraries**  
- `sklearn.decomposition.PCA`  
- `sklearn.manifold.TSNE`  
- `matplotlib.pyplot`

---

## Task 5: Apply PCA and t-SNE with 3 Components

**Description**  
- Apply PCA and t-SNE, this time reducing the data to 3 components.
- Generate 3D visualizations for both methods using the three resulting dimensions.
- Label points with class values for clarity.

**Required Libraries**  
- `sklearn.decomposition.PCA`  
- `sklearn.manifold.TSNE`  
- `matplotlib.pyplot`  
- `mpl_toolkits.mplot3d` (for 3D plotting)

---

## Task 6: Compare the Results

**Description**  
- Compare the 2D visualizations of PCA and t-SNE.
- Compare the 3D visualizations of PCA and t-SNE.
- Reflect on the following:
  - Which method best separates the data clusters?
  - Does 3D reveal structure that 2D did not?
  - Which method do you find most informative, and why?

## Task 7: Create a Composite Visualization of All Dimensionality Reduction Results

**Description**  
- Generate a figure that displays all four visualizations:
  1. PCA with 2 components
  2. t-SNE with 2 components
  3. PCA with 3 components
  4. t-SNE with 3 components
- Use subplots to arrange these plots clearly.
- Ensure that each subplot has a descriptive title and consistent coloring for labels.
- This composite view will help you and others visually compare how PCA and t-SNE perform across different dimensional settings.

**Required Libraries**  
- `matplotlib.pyplot`  
- `mpl_toolkits.mplot3d` (for 3D subplots)

---

📌 **Tip:** You can use `plt.subplots()` for 2D plots and `fig.add_subplot(projection='3d')` for 3D ones. Arrange the plots in a 2x2 grid layout for clarity.
