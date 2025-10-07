# Vendor & Inventory Analysis Project

## 📊 Project Overview

This project provides a comprehensive analysis of vendor performance, inventory management, and profitability optimization for retail and wholesale operations. The analysis identifies key opportunities for improving operational efficiency, reducing costs, and maximizing profit margins through data-driven insights.

## 🎯 Business Objectives

The primary goals of this analysis are to:

- **Identify underperforming brands** requiring promotional or pricing adjustments
- **Determine top-contributing vendors** by sales and gross profit
- **Analyze bulk purchasing impact** on unit costs and profitability
- **Assess inventory turnover** to reduce holding costs and improve efficiency
- **Investigate profitability variance** between high-performing and low-performing vendors

## 📈 Key Findings

### 1. Brand Performance & Pricing Opportunities
- **198 brands** identified with lower sales but higher profit margins
- These brands are prime candidates for targeted marketing and promotional campaigns
- Opportunity to increase sales volume without compromising profitability

### 2. Vendor Concentration Risk
- **Top 10 vendors** contribute **65.69%** of total purchases
- Remaining vendors contribute only **34.31%**
- High dependency on few vendors poses supply chain disruption risks
- **Recommendation**: Diversify vendor partnerships

### 3. Bulk Purchasing Advantages
- Large quantity orders receive **72% lower unit cost** ($10.78 vs. higher unit costs)
- Bulk pricing strategies effectively increase total sales while maintaining profitability
- **Recommendation**: Leverage bulk purchasing for competitive pricing

### 4. Inventory Management Issues
- **Total Unsold Inventory**: $2.71M in capital
- Slow-moving inventory increases storage costs and reduces cash flow
- Stock turnover ranges from 0 to 274.5 across products
- **Recommendation**: Optimize slow-moving inventory through adjusted purchasing or clearance sales

### 5. Profit Margin Analysis
- **Top Vendors**: Mean profit margin of **31.17%** (95% CI: 30.74% - 31.61%)
- **Low-Performing Vendors**: Mean profit margin of **41.55%** (95% CI: 40.48% - 42.62%)
- Low-performing vendors maintain higher margins but struggle with sales volumes
- Statistical testing confirms significant difference between vendor groups (H₀ rejected)

## 🔍 Data Analysis Highlights

### Summary Statistics Insights

**Negative Values & Losses:**
- Gross Profit minimum: **-$52,002.78** (indicating losses from discounts or selling below cost)
- Profit Margin minimum: **-∞** (instances where revenue ≤ total cost)
- Some products show **zero sales**, indicating obsolete stock

**Outliers & Variations:**
- Purchase & Actual Prices: Maximum values (5,681.81 & 7,499.99) significantly exceed means (24.39 & 35.64)
- Freight Cost: Extreme variation from $0.09 to $257,032.07
- Indicates premium products and logistics inefficiencies

### Data Filtering

To ensure data quality, the following records were excluded:
- Gross Profit ≤ 0
- Profit Margin ≤ 0
- Total Sales Quantity = 0

### Correlation Analysis

| Variables | Correlation | Insight |
|-----------|-------------|---------|
| Purchase Price vs. Sales Dollars | -0.012 | Weak - price variations don't significantly impact revenue |
| Purchase Price vs. Gross Profit | -0.016 | Weak - pricing doesn't drive profit directly |
| Purchase Quantity vs. Sales Quantity | 0.999 | Strong - efficient inventory turnover |
| Profit Margin vs. Sales Price | -0.179 | Negative - higher prices may reduce margins |
| Stock Turnover vs. Gross Profit | -0.038 | Weak - faster turnover ≠ higher profitability |

## 💡 Actionable Recommendations

### 1. Pricing Strategy Optimization
- Re-evaluate pricing for low-sales, high-margin brands
- Focus on volume growth without sacrificing profitability
- Consider dynamic pricing strategies based on market demand

### 2. Vendor Diversification
- Reduce dependency on top 10 vendors
- Develop relationships with alternative suppliers
- Mitigate supply chain disruption risks

### 3. Inventory Management
- Implement just-in-time (JIT) ordering for slow-moving items
- Launch clearance campaigns for unsold inventory worth $2.71M
- Optimize purchase quantities based on turnover rates

### 4. Vendor Performance Enhancement
- **Top Vendors**: Focus on cost efficiency and operational optimization
- **Low-Performing Vendors**: Improve marketing, distribution, and pricing strategies
- Offer bundled promotions to increase sales volume

### 5. Bulk Purchasing Leverage
- Maximize bulk purchasing discounts (72% cost reduction)
- Negotiate long-term contracts with key suppliers
- Balance inventory holding costs with unit cost savings

## 📊 Statistical Validation

**Hypothesis Testing Results:**
- **H₀**: No significant difference in profit margins between top and low-performing vendors
- **H₁**: Significant difference exists in profit margins
- **Result**: H₀ rejected - vendor groups operate under distinctly different profitability models

## 🚀 Expected Outcomes

By implementing these recommendations, the organization can achieve:

✅ Sustainable profitability through optimized pricing strategies  
✅ Reduced supply chain risks via vendor diversification  
✅ Improved cash flow through better inventory management  
✅ Enhanced operational efficiency and cost reduction  
✅ Increased sales volume without compromising margins  

## 📁 Project Structure

```

├── Exploratory Data Analysis.ipynb          # Initial EDA and data quality checks (172 KB)
├── Vendor Performance Analysis.ipynb        # Comprehensive statistical analysis (1.79 MB)
├── Vendor Performance Report.pdf            # Detailed findings and recommendations (3.02 MB)
├── vendor_performance.pbix                  # Power BI dashboard for interactive insights (1.38 MB)
├── vendor_sales_summary.csv                 # Processed vendor and sales data (2.45 MB)
└── README.md                                # Project documentation (this file)
```

### File Descriptions

**Jupyter Notebooks:**
- `Exploratory Data Analysis.ipynb` - Summary statistics, correlation analysis, and data filtering
- `Vendor Performance Analysis.ipynb` - Hypothesis testing, vendor segmentation, and profitability analysis

**Reports & Dashboards:**
- `Vendor Performance Report.pdf` - Executive summary with all key findings and recommendations
- `vendor_performance.pbix` - Interactive Power BI dashboard for real-time vendor performance monitoring

**Data:**
- `vendor_sales_summary.csv` - Consolidated dataset containing vendor transactions, inventory, and sales metrics

## 🛠️ Technologies Used

- **Data Analysis**: Python (Pandas, NumPy)
- **Statistical Testing**: SciPy, StatsModels
- **Visualization**: Matplotlib, Seaborn, Plotly
- **Reporting**: Jupyter Notebooks, Markdown

## 📧 Contact

For questions or additional information about this analysis, please contact the analytics team.

---

**Last Updated**: October 2025  
**Analysis Period**: Based on vendor and inventory data through January 2025
