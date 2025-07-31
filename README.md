# Adidas USA Product Analysis - Business Intelligence Project

## 📊 Project Overview

This comprehensive data science project analyzes Adidas USA's product portfolio using advanced machine learning techniques to extract actionable business insights. The analysis examines 845 Adidas products from the US market to identify high-performing segments, pricing strategies, and customer engagement patterns.

## 🎯 Business Objectives

- **Identify high-performing product segments** through clustering analysis
- **Analyze pricing strategies** across different demographics and categories  
- **Discover customer engagement patterns** using review and rating data
- **Provide data-driven recommendations** for portfolio optimization

## 📁 Repository Structure

```
📦 adidas-usa-analysis/
├── 📄 01_exploratory_data_analysis.ipynb          # Interactive version with Plotly graphs
├── 📄 01_exploratory_data_analysis-checkpoint.ipynb  # Static version with Matplotlib graphs
├── 📊 adidas_usa.csv                              # Dataset
└── 📖 README.md                                   # This file
```

### File Differences

- **`01_exploratory_data_analysis.ipynb`**: Contains **interactive Plotly visualizations** for dynamic exploration and web-based analysis
- **`01_exploratory_data_analysis-checkpoint.ipynb`**: Contains **static Matplotlib/Seaborn visualizations** optimized for PDF export and report generation

## 🛠️ Technical Stack & Dependencies

### Core Libraries
```python
pandas==1.4.4           # Data manipulation and analysis
numpy==1.21.5           # Numerical computations
matplotlib>=3.5.0       # Static plotting
seaborn>=0.11.0         # Statistical visualization
plotly>=5.0.0           # Interactive visualizations
```

### Machine Learning
```python
scikit-learn>=1.0.0     # ML algorithms and preprocessing
xgboost>=1.5.0          # Gradient boosting
```

### Additional Tools
```python
jupyter>=1.0.0          # Notebook environment
ipython>=7.0.0          # Enhanced Python shell
```

## 🔬 Methodology & Techniques

### 1. **Data Preprocessing & Quality**
- **Missing Value Imputation**: Random Forest-based imputation achieving 99% accuracy (R²=0.99)
- **Outlier Detection**: IQR method for identifying price and engagement anomalies
- **Feature Engineering**: Price discounts, gender classification, performance scores

### 2. **Machine Learning Applications**

#### **Missing Value Imputation**
- **Random Forest Regression**: For missing original prices (MAE: $2.24, R²: 0.99)
- **Linear Regression**: Baseline comparison (R²: 0.97)
- **Category Average**: Simple imputation method (R²: 0.37)

#### **Classification Models**
- **Random Forest**: Gender prediction (73% accuracy)
- **XGBoost**: Alternative classification approach (71% accuracy)  
- **SVM & Naive Bayes**: Comparison baselines
- **Feature Set**: Numerical, categorical, and TF-IDF text features (56 total features)

#### **Customer Segmentation**
- **K-Means Clustering**: Product performance segmentation
- **Elbow Method**: Optimal cluster determination
- **StandardScaler**: Feature normalization for clustering

### 3. **Statistical Analysis**
- **Correlation Analysis**: Feature relationship exploration
- **Box Plots & Violin Plots**: Distribution analysis
- **Outlier Analysis**: Business vs. statistical anomaly identification

## 📈 Key Findings

### Market Segmentation Results
1. **Premium Moderate Performers** (19.5%): High-priced ($100 avg) with moderate engagement
2. **Star Products** (1.5%): Mid-priced ($47 avg) with exceptional engagement (8,659 reviews avg)
3. **Average Performers** (20.2%): Mid-range pricing with low engagement  
4. **Budget Mass Market** (58.7%): Low-priced products with modest performance

### Business Insights
- **Category Dominance**: All top 20 best-sellers are shoes
- **Gender Strategy**: Men generate 48.7% revenue despite 41% product share
- **Pricing Consistency**: 22% average discount across all segments

## 🚀 Strategic Recommendations

### Immediate Actions (0-3 months)
1. **Star Product Replication**: Analyze Stan Smith & Superstar success factors
2. **Men's Portfolio Expansion**: Increase premium men's products

### Medium-term Strategy (3-12 months)  
3. **Category Diversification**: Apply shoe success to clothing/accessories
4. **Women's Market Enhancement**: Address satisfaction gap (4.57 vs 4.70 rating)

### Expected Impact
- **Revenue Growth**: 15-20% potential increase
- **Market Position**: Enhanced competitive positioning in premium segments

## 📊 Dataset Information

- **Size**: 845 products × 21 features
- **Source**: Kaggle Dataset - Web-scraped e-commerce data (October 2021)
- **Coverage**: US market Adidas products
- **Categories**: Shoes, Clothing, Accessories
- **Demographics**: Men, Women, Kids

**Dataset Credit**: https://www.kaggle.com/datasets/thedevastator/adidas-fashion-retail-products-dataset-9300-prod/data

## 🔧 Setup & Installation

```bash
# Clone repository
git clone https://github.com/your-username/adidas-usa-analysis.git
cd adidas-usa-analysis

# Install dependencies
pip install pandas==1.4.4 numpy==1.21.5 matplotlib seaborn plotly scikit-learn xgboost jupyter

# Launch Jupyter
jupyter notebook
```

## 📋 Usage

1. **For Interactive Analysis**: Open `01_exploratory_data_analysis.ipynb`
2. **For Static Reports**: Open `01_exploratory_data_analysis-checkpoint.ipynb`
3. **Run All Cells**: Execute sequentially for complete analysis

## 🤝 Contributing

Feel free to submit issues, feature requests, or pull requests to improve this analysis.

## 📄 License & Usage

- **Code**: Free to use for educational and research purposes
- **Dataset**: Please refer to original Kaggle dataset terms and conditions
- **Commercial Use**: Contact for permissions

## 🙏 Acknowledgments

- Dataset provided by The Devastator on Kaggle
- This project was completed as part of Industrial Engineering & Management - Data Science track

---
## Dashboard Preview
https://public.tableau.com/views/Book2_17539981268580/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
<img width="999" height="799" alt="Dashboard 1" src="https://github.com/user-attachments/assets/1e05b94a-a6de-4284-841b-3fa953067eb9" />

*This analysis demonstrates advanced data science techniques applied to real-world business problems, providing actionable insights for strategic decision-making.*
