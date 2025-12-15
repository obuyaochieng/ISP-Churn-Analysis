# ISP Customer Churn Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![PowerBI](https://img.shields.io/badge/PowerBI-Visualization-yellow)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Complete-success)

## 📋 Overview
This project analyzes customer churn for an Internet Service Provider (ISP) using the IBM Telco Customer Churn dataset. The analysis identifies key factors driving customer attrition and provides actionable insights for improving retention strategies.

**Key Features:**
- 📊 **Comprehensive EDA** with statistical analysis
- 🧹 **Data cleaning** and preprocessing pipeline
- 📈 **Interactive Power BI dashboards** for business insights
- 🔍 **Churn driver identification** across multiple dimensions
- 💡 **Actionable recommendations** for reducing churn

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Power BI Desktop (for visualization)
- Git

### Installation
```bash
# Clone the repository
git clone https://github.com/obuyaochieng/isp-churn-analysis.git

# Navigate to project directory
cd isp-churn-analysis

# Install required Python packages
pip install -r requirements.txt
```

### Run the Analysis
1. **Data Preparation:**
   ```bash
   # The processed dataset is available in data/processed/
   # To regenerate from raw data, run all cells in the notebook
   ```

2. **Execute Jupyter Notebook:**
   ```bash
   jupyter notebook CustomeISPchurn.ipynb
   ```

3. **View Power BI Dashboard:**
   - Open `powerbi/churn_dashboard.pbix` in Power BI Desktop
   - Refresh data connections if needed

## 📁 Project Structure
```
isp-churn-analysis/
├── data/
│   ├── raw/                    # Original dataset (not in repo - download separately)
│   └── processed/              # Cleaned dataset (7032 rows × 21 columns)
│       └── churn_data_cleaned.csv
├── notebooks/
│   └── CustomeISPchurn.ipynb   # Main analysis notebook
├── powerbi/
│   └── churn_dashboard.pbix    # Interactive Power BI dashboard
├── docs/
│   └── analysis_report.pdf     # Detailed analysis report
├── requirements.txt            # Python dependencies
├── .gitignore                  # Git ignore file
└── README.md                   # This file
```

## 📊 Key Insights

### Churn Distribution
- **Overall Churn Rate:** 26.58% 
- **Retention Rate:** 73.42%
- Significant revenue opportunity in reducing churn

### Top Churn Drivers Identified:
1. **Contract Type:** Month-to-month customers → 42.7% churn rate
2. **Tenure:** New customers (<12 months) → 41.5% churn rate  
3. **Payment Method:** Electronic check users → 33.6% churn rate
4. **Service Features:** No tech support → 29.4% churn rate
5. **Monthly Charges:** >$70/month → 32.8% churn rate

### Power BI Dashboard Features:
- **Executive Summary:** High-level churn metrics
- **Customer Segmentation:** Demographic & behavioral analysis
- **Risk Scoring:** Predictive churn likelihood
- **Financial Impact:** Revenue at risk calculations
- **Interactive Filters:** Drill-down capabilities

## 🛠️ Technologies Used

**Data Analysis:**
- Python 3.8+
- Pandas & NumPy (data manipulation)
- Matplotlib & Seaborn (visualization)
- Jupyter Notebooks

**Business Intelligence:**
- Power BI Desktop
- DAX calculations
- Interactive visualizations

**Version Control:**
- Git & GitHub

## 📈 Results & Recommendations

### Immediate Actions:
1. **Target high-risk segments** with personalized retention offers
2. **Implement early-warning system** for at-risk customers
3. **Improve onboarding process** for new customers

### Strategic Initiatives:
1. **Promote annual contracts** with incentives
2. **Bundle essential services** to increase stickiness
3. **Encourage automatic payments** to reduce friction

### Long-term Solutions:
1. **Develop predictive models** for proactive intervention
2. **Create customer success programs** for key segments
3. **Establish feedback loops** for continuous improvement

## 📚 Dataset Information

**Source:** IBM Telco Customer Churn Dataset  
**Initial Records:** 7,043 customers  
**Cleaned Records:** 7,032 customers  
**Features:** 21 variables including:
- Customer demographics (gender, senior citizen, partner, dependents)
- Account information (tenure, contract type, payment method)
- Service subscriptions (internet, phone, streaming, security)
- Billing details (monthly charges, total charges)
- Target variable: Churn (Yes/No)

## 🎯 Usage Examples

### For Data Scientists:
```python
# Load cleaned dataset
import pandas as pd
df = pd.read_csv('data/processed/churn_data_cleaned.csv')

# Explore churn distribution
churn_rate = df['Churn'].value_counts(normalize=True) * 100
print(f"Churn Rate: {churn_rate['Yes']:.2f}%")
```

### For Business Analysts:
- Use Power BI dashboard for ad-hoc analysis
- Filter by customer segments to identify patterns
- Export reports for stakeholder presentations

### For Decision Makers:
- Review executive summary in Power BI
- Monitor key churn metrics monthly
- Implement recommended retention strategies

## 🔄 Development Workflow

1. **Data Collection:** IBM Telco dataset
2. **Data Cleaning:** Handle missing values, convert data types
3. **Exploratory Analysis:** Identify patterns and correlations
4. **Insight Generation:** Determine churn drivers
5. **Visualization:** Create Power BI dashboards
6. **Reporting:** Document findings and recommendations

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

Project Link: https://github.com/obuyaochieng/isp-churn-analysis](https://github.com/obuyaochieng/isp-churn-analysis)

## 🙏 Acknowledgments

- IBM for providing the Telco Customer Churn dataset
- Open-source community for Python data science libraries
- Contributors and reviewers

## 📊 Sample Visualizations

![Churn Distribution](https://via.placeholder.com/800x400.png?text=Churn+Distribution+Chart)
![Tenure Analysis](https://via.placeholder.com/800x400.png?text=Tenure+vs+Churn+Analysis)

---

⭐ **If you find this project useful, please give it a star!** ⭐