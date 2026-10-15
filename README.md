# Market Basket Analysis

## Overview
An association-rule mining project that identifies products commonly purchased together and translates them into cross-selling recommendations.

## Dataset
UCI Machine Learning Repository — Online Retail  
https://archive.ics.uci.edu/dataset/352/online+retail  
Citation: Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33.

The notebook downloads the official UCI ZIP containing the Excel data when run in an internet-enabled environment. If automatic download fails, download `Online Retail.xlsx` from the UCI page and upload it beside the notebook.

## Run in Google Colab
1. Upload `Market_Basket_Analysis.ipynb` to Google Colab.
2. Uncomment and run the dependency installation line if required.
3. Run cells from top to bottom. The dataset is large, so allow time for loading and Apriori analysis.
4. Review the top products, frequent itemsets, association rules, and visualizations.
5. Download the `outputs/` folder for your portfolio.

## Methodology
- Remove missing records, cancellation invoices, non-positive quantities/prices, and non-product charges.
- Focus the initial basket analysis on UK transactions.
- Encode invoice-product combinations as a boolean basket matrix.
- Apply Apriori to find frequent itemsets.
- Generate rules and rank them using support, confidence, and lift.

## Tools
Python, Pandas, NumPy, Matplotlib, Seaborn, Mlxtend, OpenPyXL.

## Repository structure
```text
market_basket_analysis/
├── Market_Basket_Analysis.ipynb
└── README.md
```

## Suggested GitHub repository description
Market basket analysis on UCI Online Retail data using Apriori, frequent itemsets, and association rules to support cross-selling.

## Limitations
The analysis is observational and does not establish causation. The dataset is historical and specific to one retailer. Test recommendations before implementing them commercially.
