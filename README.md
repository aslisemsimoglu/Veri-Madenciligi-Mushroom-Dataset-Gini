# 🍄 Mushroom Classification Project 🌟

## 📌 About the Project
This project aims to classify mushrooms as **edible** or **poisonous** based on their physical and chemical characteristics. Using the **Gini Index** algorithm, we built a decision tree model and performed detailed analyses on the dataset's features. The project highlights key data mining techniques and serves as a practical application of classification models. 🚀

---

## 🎯 Project Goals
- Explore the relationship between mushrooms' attributes and their edibility.
- Build a high-accuracy classification model by analyzing the dataset's features.
- Develop skills in processing and analyzing large datasets using data mining techniques.

---

## 👩‍💻 Team Members
This project was developed as part of the **Data Mining Course** in the Department of Computer Engineering at Afyon Kocatepe University by:

- 🌟 **Aslı Şemşimoğlu**
- 🌟 **Rabia Durgut**
- 🌟 **Rabia Ebrar Dal**

---

## 📂 Dataset Overview: Mushroom Dataset
- **Total Records**: 8,124  
- **Features**: 23  
- **Target Variable**: `class` (edible: `e`, poisonous: `p`)  

Dataset Link: [Kaggle Mushroom Dataset](https://www.kaggle.com/uciml/mushroom-classification)

---

## 🔍 Steps and Workflow
### 1️⃣ Data Exploration
We analyzed the dataset's structure, unique values, and missing data:
- **Total Features**: 23  
- **Unique Values Per Feature**: Extracted for understanding categorical variety.  
- **Missing Data**: Identified and processed.

### 2️⃣ Data Cleaning
- Removed unnecessary columns (e.g., `veil-type`, which contains a single unique value).
- Treated missing values in `stalk-root` as a separate category.

### 3️⃣ Data Transformation
- Applied **Label Encoding** to convert categorical variables into numerical representations for compatibility with machine learning models.

### 4️⃣ Train-Test Split
- Split the dataset into training (80%) and testing (20%) sets to evaluate model performance.

### 5️⃣ Decision Tree Construction
- Built a decision tree using the **Gini Index** to determine the best split points.  
- Recursively partitioned the dataset to create an optimized tree structure.  

### 6️⃣ Model Evaluation
- Assessed the model's accuracy on the test set: **95%**.
- Visualized the decision tree and classification results using bar plots and confusion matrices.

---

## 🌟 Key Features
1. **Gini Index Calculation**:  
   Measured group purity and determined the best split points.
2. **Custom Decision Tree Construction**:  
   Built a recursive algorithm for creating decision trees from scratch.
3. **Visualization**:  
   Used graphs, heatmaps, and bar charts to analyze results effectively.
4. **Classification Analysis**:  
   Identified misclassified samples and examined reasons for inaccuracies.

---

## 🖥️ Example Code

### Load and Explore Data
```python
import pandas as pd

# Load dataset
data = pd.read_csv('/kaggle/input/mushroom-classification/mushrooms.csv')

# Overview of data
print(data.info())
print(data.head())
