# 💡 **Customer Feedback and Production Efficiency Analysis on DataCo Smart Supply Chain**

### **Created by:**
- Winston Narada Kusumahadi
- Bryant Gabriel Effendi
- Farrany Sucitra Kusumahadi

## 📑 **Project Description**
This project aims to analyze customer feedback and production efficiency in **DataCo Smart Supply Chain**. By leveraging the available data, this project evaluates the quality of delivery services and models customer clustering as well as production efficiency.

### 🎯 **Main Objectives:**
1. Cluster customers based on their characteristics and feedback.
2. Measure delivery efficiency by calculating *Mean Absolute Percentage Error* (MAPE).
3. Calculate the risk of delivery delays using *Log Loss*.
4. Identify relationships between variables through data exploration.

---------------------------------------------------------

## ⚙️ **Techniques and Models Used**

### 🔍 **1. Exploratory Data Analysis (EDA)**
- Perform descriptive statistical analysis to understand data distribution.
- Identify missing values (*missing values*) and outliers.
- Visualize data using *heatmaps* and *histograms* to map feature correlations.

### 🧠 **2. Clustering with K-Means**
- Use *K-Means Clustering* to group data based on feature similarities.
- Evaluate clustering results using the following metrics:
  - **Davies-Bouldin Index:** Measures how well clusters are formed.
  - **Calinski-Harabasz Index:** Measures cluster density and separation.

### 📈 **3. Model Evaluation**
- Calculate **MAPE (Mean Absolute Percentage Error)** to predict delivery efficiency.
- Calculate **Log Loss** to estimate the risk of delivery delays.

### 🗃️ **4. Dimensionality Reduction with PCA**
- Use *Principal Component Analysis (PCA)* to reduce data dimensions for 2D visualization.

---------------------------------------------------------

## 📝 **Project Structure**
```bash
├── data.ipynb                 # Main notebook for data analysis
├── data/                      # Dataset folder
│   ├── Dataset_Pertama.csv
│   └── Dataset_Kedua.csv
├── models/                    # Folder to store trained models
│   ├── kmeans_model.pkl
│   └── scaler.pkl
├── results/                   # Folder for clustering and analysis results
│   └── hasil_clustering.csv
├── README.md                  # Project documentation
```

---------------------------------------------------------

## 🚀 **How to Run the Project**

### ✅ **Requirements:**
Make sure you have Python version 3.8 or newer.

### 🔧 **1. Clone the Repository:**
```bash
git clone https://github.com/username/DataCo-SupplyChain-Analysis.git
cd DataCo-SupplyChain-Analysis
```

### 📦 **2. Install Required Libraries:**
```bash
pip install pandas
pip install numpy
pip install seaborn
pip install matplotlib
pip install scikit-learn
pip install joblib
```

### ▶️ **3. Run the Analysis:**
The data is processed and analyzed within the data.ipynb notebook.

## 📂 **4. Output**
After running the code, you will obtain several output files, including:

- **hasil_clustering.csv:** Clustering results with cluster labels.
- **kmeans_model.pkl:** Trained *K-Means* model.
- **scaler.pkl:** *Standard Scaler* model used.
- **Graphical Visualizations:** Clustering and correlation charts saved as images.

## 📊 **5. Evaluation Results**
The following are the evaluation results of clustering and prediction:

- **Davies-Bouldin Index:** Measures cluster validity (lower is better).
- **Calinski-Harabasz Index:** Measures cluster separation (higher is better).
- **MAPE (Mean Absolute Percentage Error):** Measures prediction accuracy for delivery time.
- **Log Loss:** Measures the risk of delivery delays.

---

## 📚 **References**
Documentation for libraries used in this project:
- [Scikit-learn Documentation](https://scikit-learn.org/)
- [Pandas Documentation](https://pandas.pydata.org/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Joblib Documentation](https://joblib.readthedocs.io/)
