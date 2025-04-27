# Credit Card Customer Segmentation

This project aims to perform customer segmentation analysis on credit card users to identify distinct customer groups based on their behavior and characteristics. The analysis uses unsupervised machine learning techniques, specifically K-means clustering, to group customers into meaningful segments.

## Project Overview

The project analyzes various customer attributes such as spending behavior, credit limits, payment patterns, and other relevant features to identify natural groupings of customers. This segmentation can help in:

- Developing targeted marketing strategies
- Improving customer service
- Risk management
- Product development
- Understanding customer behavior patterns

## Setup

1. This project uses Poetry for dependency management. Ensure you have Poetry installed:

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

2. Install dependencies:

```bash
poetry install
```

3. Activate the virtual environment:

```bash
source .venv/bin/activate
```

## Dependencies

- pandas - Data manipulation and analysis
- numpy - Numerical computations
- matplotlib - Data visualization
- seaborn - Statistical data visualization
- scikit-learn - Machine learning algorithms
- jupyter - Interactive notebook environment

## Project Structure

- `credit_card_customer_segmentation.ipynb` - Main Jupyter notebook containing the analysis
- `customer_segmentation.csv` - Dataset containing customer information
- `data_dictionary.md` - Detailed description of dataset features and their meanings
- `dataset_documentation.ipynb` - Additional documentation and exploratory analysis of the dataset
- `README.md` - Project documentation
- `pyproject.toml` & `poetry.lock` - Poetry dependency management configuration
- `project_info.txt` - Additional project notes and information

## Documentation

For a detailed understanding of the dataset features and their meanings, please refer to:
1. `data_dictionary.md` - Contains definitions of all variables in the dataset
2. `dataset_documentation.ipynb` - Provides in-depth analysis and examples of the data structure

## Analysis Steps

1. Data Loading and Exploration
2. Data Preprocessing and Feature Engineering
3. Feature Scaling
4. K-means Clustering
5. Cluster Analysis and Interpretation
6. Visualization of Results

## Usage

To run the analysis:

1. Ensure you're in the virtual environment:
```bash
source .venv/bin/activate
```

2. Launch Jupyter notebook:
```bash
poetry run jupyter notebook
```

3. Open `credit_card_customer_segmentation.ipynb` in the Jupyter interface
