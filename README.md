# 🧹 Data Wrangling Labs – Car & Laptop Datasets

This repository contains my data wrangling labs, where I worked with **real-world datasets (cars and laptops)** and applied various preprocessing techniques to clean, standardize, and prepare the data for **exploratory analysis and machine learning models**.  

---

## 📂 Contents
- `Car Data_Analysis.ipynb` → Data wrangling and analysis on automobile dataset.  
- `Laptop Data_Analysis.ipynb` → Data wrangling and analysis on laptop dataset.  
- `Laptop_DataSet.csv` → Cleaned version of the Laptop dataset.  
- `cleaned dataset.csv` → Cleaned version of the automobile dataset after applying transformations.  
- `README.md` → Project documentation.  

---

## 📊 Dataset Descriptions

### 🚗 Car Dataset
- **Notebook:** `Car Data_Analysis.ipynb`  
- **Cleaned version saved as:** `cleaned dataset.csv`  
- **Attributes include:** `make`, `fuel-type`, `aspiration`, `horsepower`, `price`, etc.  
- **Use case:** Useful for predicting car prices, analyzing market segments, and preparing data for regression/classification models.

### 💻 Laptop Dataset
- **Notebook:** `Laptop Data_Analysis.ipynb`  
- **Raw dataset file:** `Laptop_DataSet.csv`  
- **Cleaned version saved as:** `cleaned dataset.csv`  
- **Attributes include:** `Brand`, `Model`, `Screen_Size_cm`, `Weight_kg`, `Processor`, `RAM`, `Price`, etc.  
- **Use case:** Standardizing laptop specifications, comparing products globally, and preparing features for recommendation or prediction systems.

---

## 🛠 Techniques Applied

### 1. Handling Missing Data
- **What I did:**  
  - Detected missing values.  
  - Replaced them with mean/median (for numeric data) or most frequent values (for categorical data).  
- **Why:**  
  - Missing data causes errors in analysis & models.  
  - Ensures dataset is consistent and usable for training ML models.

---

### 2. Data Type Conversion
- **What I did:**  
  - Converted `price` and `horsepower` from `object` → `float`.  
  - Ensured categorical columns like `fuel-type` were stored as `category`.  
- **Why:**  
  - Correct data types are critical for numeric operations and memory efficiency.  
  - Prevents errors during visualization and ML preprocessing.

---

### 3. Standardization & Unit Conversion
- **Laptop dataset:**  
  - Converted **weight** from `kg → pounds`.  
  - Converted **screen size** from `cm → inches`.  
- **Why:**  
  - Makes data consistent across sources (e.g., some countries use inches, some use cm).  
  - Helps comparison of products in global datasets.  

---

### 4. Normalization
- **Car dataset:**  
  - Normalized numerical features like `length`, `width`, and `height` to a range [0,1].  
- **Why:**  
  - Brings all numerical features to the same scale.  
  - Prevents bias in ML models where features with larger values dominate.

---

### 5. Binning
- **Car dataset:**  
  - Grouped `horsepower` into bins: `Low`, `Medium`, `High`.  
- **Why:**  
  - Simplifies continuous data into categories for analysis.  
  - Makes it easier to study customer segments (e.g., economy vs. sports cars).  

---

### 6. Dummy Variables (One-Hot Encoding)
- **Car dataset:**  
  - Converted categorical variables (`fuel-type`, `aspiration`, etc.) into binary columns.  
- **Why:**  
  - Many ML algorithms cannot work directly with text categories.  
  - Encoding ensures categorical features are machine-readable.

---

### 7. Feature Engineering
- **Laptop dataset:**  
  - Created new features like `Screen_Size_inch` and `Weight_pounds`.  
- **Why:**  
  - Derived attributes provide more meaningful insights.  
  - Helps in comparing laptops and feeding standardized features into models.

---

## 🚀 Applications of These Techniques in Real-World Projects

- **Car dataset techniques:**  
  - Price prediction models.  
  - Customer segmentation (low/mid/high horsepower).  
  - Market trend analysis for automobile companies.  

- **Laptop dataset techniques:**  
  - Product comparison engines.  
  - Standardized specifications for recommendation systems.  
  - Better data integration across global e-commerce platforms.  

---

## 🧰 Tools & Libraries
- Python 3.x  
- Jupyter Notebook  
- Pandas  
- NumPy  
- Matplotlib  

---

## 🔑 Learning Outcomes
Through these labs, I gained hands-on experience with:  
- Data cleaning (missing values, incorrect types).  
- Standardization and normalization.  
- Binning and categorical encoding.  
- Feature engineering.  
- Preparing datasets for visualization and machine learning.  

---

## 📌 Notes
- Car dataset is analyzed in `Car Data_Analysis.ipynb` and cleaned version is stored in `cleaned dataset.csv`.  
- Laptop dataset is analyzed in `Laptop Data_Analysis.ipynb`, and cleaned version is also stored in `cleaned dataset.csv`.  
- This work is part of my **Data Science coursework on Coursera**.  
