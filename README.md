# Developing a Recommendation System using Association Rule Mining (FP-Growth) on E-commerce Data

This project implements a recommendation system for e-commerce using the FP-Growth algorithm for association rule mining. The analysis is performed on the Instacart Market Basket dataset.

## Project Structure

```
├── notebooks/
│   ├── Exploritory_Data_Analysis.ipynb    # EDA and data preprocessing
│   ├── Market_Basket_Analysis.ipynb       # FP-Growth implementation
│   └── Evaluation_Business_Insights.ipynb # Results analysis and insights
├── outputs/
│   ├── association_rules.csv              # Generated association rules
│   ├── cross_dept_association_rules.csv   # Cross-department rules
│   ├── clean_transactions.pkl             # Processed transaction data
│   └── images/                            # Visualization outputs
└── data/                                  # Dataset (not included in repo)
```

## Setup

### Prerequisites
- Python 3.13+
- Virtual environment (recommended)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Feketebalazs/Developing-a-Recommendation-System-using-Association-Rule-Mining-FP-Growth-on-E-commerce-Data.git
cd Developing-a-Recommendation-System-using-Association-Rule-Mining-FP-Growth-on-E-commerce-Data
```

2. Create and activate virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn mlxtend jupyter ipywidgets
```

### Dataset

Download the Instacart Market Basket Analysis dataset from [Kaggle](https://www.kaggle.com/c/instacart-market-basket-analysis/data) and place the CSV files in the `data/` directory.

Required files:
- `orders.csv`
- `order_products_prior.csv`
- `order_products_train.csv`
- `products.csv`
- `aisles.csv`
- `departments.csv`

## Usage

Run the notebooks in order:

1. **Exploratory Data Analysis**: Analyzes the dataset and performs data preprocessing
2. **Market Basket Analysis**: Implements FP-Growth algorithm and generates association rules
3. **Evaluation & Business Insights**: Evaluates rules and provides actionable business insights

## Key Features

- Memory-optimized data loading for large datasets
- FP-Growth algorithm for efficient frequent itemset mining
- Association rule generation with configurable support and confidence thresholds
- Cross-department product recommendations
- Business insights and actionable recommendations

## Results

The analysis generates:
- Association rules with support, confidence, and lift metrics
- Cross-departmental product associations
- Visualization of key patterns and insights
- CSV exports for further analysis

## License

This project is for educational purposes.

## Acknowledgments

- Dataset: Instacart (via Kaggle)
- Algorithm: FP-Growth implementation using mlxtend library
