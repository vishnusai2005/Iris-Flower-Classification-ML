# Iris-Flower-Classification-ML
# Iris Flower Classification using K-Nearest Neighbors (KNN)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit_Learn-orange.svg)
![Jupyter](https://img.shields.io/badge/Tool-Jupyter_Notebook-F37626.svg)

##  Project Overview
The objective of this project is to build a Machine Learning model that can accurately classify a new Iris flower into one of three species: **Setosa, Versicolour, or Virginica**. This classification relies on the morphological features of the flowers and is implemented using the K-Nearest Neighbors (KNN) algorithm.

##  Dataset
The project uses the classic **Iris Dataset** (`IRIS.csv`), which consists of 150 samples of iris flowers, evenly distributed across the three species.

**Features (in centimeters):**
- `sepal_length`
- `sepal_width`
- `petal_length`
- `petal_width`

**Target Variable:**
- `species` (Iris-setosa, Iris-versicolor, Iris-virginica)

##  Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Checked for missing values to ensure data integrity.
- Visualized feature relationships using Scatter plots, Seaborn FacetGrids, KDE plots, and Boxplots to understand the distribution, detect outliers, and observe how species cluster based on dimensions.
- Utilized Pairplots to analyze pairwise relationships between all numerical features.

### 2. Data Preprocessing
- Separated the dataset into independent features (`X`) and the target variable (`y`).
- Split the data into an 80/20 train-test split for unbiased evaluation.

### 3. Model Building & Evaluation
- Initialized a baseline KNN Classifier using the Euclidean distance metric.
- Evaluated the model achieving **100% accuracy** on the test set.
- Generated a Confusion Matrix and Classification Report for detailed metric analysis (Precision, Recall, F1-score).

### 4. Hyperparameter Tuning
- Conducted an iterative test for `K` values ranging from 1 to 20 to ensure model robustness.
- Applied the **Elbow Method** (K-Value vs. Accuracy curve) to visually identify the optimal number of neighbors.
- Selected `k=15` as the final, highly stable parameter.

### 5. Final Prediction
- Retrained the final model using the entire dataset with `n_neighbors=15`.
- Successfully classified an unseen, custom flower sample `[4.5, 3.1, 1.7, 0.6]` as **Iris-setosa**.

## 💻 Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
   cd your-repo-name
