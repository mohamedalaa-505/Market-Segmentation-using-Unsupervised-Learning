# 📊 Market Segmentation using Unsupervised Learning

## 📌 Overview
This project applies an end-to-end **machine learning pipeline** to identify key customer segments for a German mail-order company.  
The goal is to determine which individuals in the general population are most likely to become customers, enabling more efficient and targeted marketing.

---

## ⚙️ Project Pipeline
The analysis follows a structured six-step workflow:

1. **Data Exploration & Preprocessing**  
   - Load datasets  
   - Analyze missing values  
   - Clean and prepare data  

2. **Feature Engineering & Encoding**  
   - Convert categorical features into numerical format  
   - Create derived features  

3. **Feature Scaling**  
   - Standardize data for better model performance  

4. **Dimensionality Reduction (PCA)**  
   - Reduce feature space while preserving variance  

5. **Clustering (K-Means)**  
   - Segment population and customers into **7 clusters**  

6. **Market Profiling**  
   - Compare clusters to identify target customer segments  

---

## 🗂️ Datasets

| Dataset | Description |
|--------|------------|
| **Udacity_AZDIAS_Subset.csv** | General population data (891,221 rows × 85 features) |
| **Udacity_CUSTOMERS_Subset.csv** | Customer data (191,652 rows × 85 features) |
| **AZDIAS_Feature_Summary.csv** | Feature metadata and descriptions |

---

## 📈 Key Results

### 🎯 Target Segment — Cluster 0
This cluster is **overrepresented among customers**, making it the ideal target group.

**Characteristics:**
- 🚗 High car ownership density *(+76.35 vs population mean)*  
- 👤 Mature life stage *(+9.44)*  
- 🔄 High mobility *(+1.20)*  
- 🌱 Preference for avantgarde & green lifestyles *(+0.74)*  

---

### 🚫 Non-Target Segment — Cluster 6
This cluster is **underrepresented** and unlikely to convert into customers.

**Characteristics:**
- 🏙️ Urban, low car ownership *(-54.63)*  
- 💸 Lower financial engagement  
- 🧍 Less consumption-driven behavior  

---

## 🧠 Conclusion
The clustering model successfully identifies distinct population segments, allowing the company to:

- 🎯 Focus on high-potential customers  
- 💰 Reduce marketing costs  
- 📊 Improve campaign efficiency  

---

## 🛠️ Technologies Used
- Python  
- Pandas & NumPy  
- Scikit-learn  
- Matplotlib & Seaborn  

---

## 🚀 How to Run
```bash
# Clone the repository
git clone https://github.com/your-username/market-segmentation.git

# Navigate to the project folder
cd market-segmentation

# Run the notebook
jupyter notebook
