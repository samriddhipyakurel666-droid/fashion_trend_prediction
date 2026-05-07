# Fashion Trend Prediction with Decision Trees 👗👕

## 📌 Overview
This project uses machine learning in R to predict whether a clothing item is **trending** based on its category, gender, price, and ratings.  
The model is built using a **Decision Tree Classifier** (`rpart`) and visualized with `rpart.plot`.  
The goal is to provide interpretable AI insights into fashion trends, with clear visualizations that highlight how decisions are made.

---

## 📂 Dataset
- **Source**: [Myntra Fashion Dataset on Kaggle](https://www.kaggle.com)  
- **Size**: ~500,000 rows (recommended sample: 10,000 rows for faster computation).  
- **Key Columns**:
  - `BrandName`
  - `Individual_category` (e.g., Jeans, T-shirts, Kurtas)
  - `category_by_Gender` (Men/Women)
  - `OriginalPrice`
  - `Ratings`

**Target Variable**:  
- A new column `Is_Trending` is created:
  - If `Ratings > 4.2` → `"Yes"`
  - Else → `"No"`

This transforms the problem into a **classification task**.

---

## 🤖 Model
- **Algorithm**: Decision Tree Classifier (`rpart`)  
- **Why Decision Trees?**
  - Simple and interpretable.  
  - Handles both categorical and numerical data.  
  - Produces a flowchart visualization that explains the AI’s decision-making process.  

**R Packages Used**:
- `tidyverse` → Data cleaning & visualization  
- `rpart` → Decision Tree model  
- `rpart.plot` → Flowchart visualization  

---

## ⚙️ Installation
Clone the repository and install required packages in R:

```bash
git clone https://github.com/your-username/fashion-trend-prediction.git
cd fashion-trend-prediction
