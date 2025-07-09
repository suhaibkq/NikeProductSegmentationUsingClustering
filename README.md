# 👟 Product Segmentation — Nike vs Adidas

## 📌 Problem Statement

### 🧠 Business Context

When planning for a trip, having the right footwear is critical—and the top two brands that come to mind are Nike and Adidas. As part of a market research company, you have been tasked with analyzing a dataset of shoes from both brands. The goal is to group products based on their features and extract insights to support marketing, pricing, and inventory strategies.

## 🎯 Objective

- Perform exploratory data analysis (EDA) on product listings
- Cluster products based on numerical and categorical features
- Identify meaningful product segments to inform business decisions

## ❓ Key Questions

- Which variables are most important for product clustering?
- How do product clusters differ from each other?
- What business recommendations can be drawn from the clustering?

## 📊 Dataset Overview

- **File**: `data_add_nik.csv`
- **Size**: 3268 rows
- **Columns**:
  - `Product Name`: Name of the product
  - `Product ID`: Unique ID
  - `Listing Price`: Original price before discount
  - `Sale Price`: Discounted selling price
  - `Discount`: Percentage discount offered
  - `Brand`: Nike or Adidas
  - `Rating`: Average customer rating
  - `Reviews`: Number of customer reviews

## 📁 Repository Structure

```
├── ML_W3_AdditionalCaseStudy_ProductSegmentation_.ipynb   # Main notebook
├── data_add_nik.csv                                       # Dataset
├── README.md                                              # Project documentation
```

## 🔍 Project Workflow

1. **Data Cleaning & Preprocessing**
   - Removed duplicates and handled null values
   - Converted percentage strings to numerical format
   - Feature engineering to calculate effective discount and review score

2. **Exploratory Data Analysis**
   - Compared pricing and rating trends between Nike and Adidas
   - Visualized product distribution by brand and discount tiers

3. **Feature Scaling & Selection**
   - Scaled continuous variables using StandardScaler
   - Selected key features for clustering (e.g., `Sale Price`, `Discount`, `Rating`, `Reviews`)

4. **Clustering Techniques**
   - Used **KMeans** clustering to segment products
   - Determined optimal number of clusters using the Elbow Method
   - Interpreted cluster profiles based on average feature values

## 🏆 Results & Insights

- **Key Finding**: Product ratings and discount levels were strong differentiators
- **Nike vs Adidas**: Nike had more premium products; Adidas offered deeper discounts
- **Clusters Identified**:
  - Budget-friendly highly rated items
  - Expensive but low-rated items
  - High-end premium segment

## 📈 Business Recommendations

- Use high-discount clusters to drive flash sales
- Upsell mid-range products that fall between budget and premium
- Leverage cluster insights to tailor marketing messages for each customer segment

## 🚀 Future Enhancements

- Apply **Hierarchical Clustering** for more nuanced segments
- Use NLP to analyze product names and descriptions
- Create interactive dashboards using Plotly or Tableau

## 👨‍💻 Author

**Suhaib Khalid**  
ML Practitioner

