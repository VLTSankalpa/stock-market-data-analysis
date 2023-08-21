# **Stock Market Data Analysis - Estimating Shares Outstanding**

Predicting the number of shares outstanding for publicly listed companies is crucial for a variety of financial analyses and investment decisions. Shares outstanding represent the total number of shares held by all of a company's shareholders, including insiders, and are a key metric in understanding a company's ownership structure. By accurately predicting the shares outstanding, investors can assess a company's market capitalization, earnings per share, and other fundamental ratios, making it an essential part of stock valuation and financial planning.

In this repository, we focus on estimating the number of shares outstanding for publicly listed companies using stock market data. We leverage metrics extracted from SEC 10K fillings, as provided in the **`fundamentals.csv`** file from the **[New York Stock Exchange (S&P 500 companies historical prices with fundamental data)](https://www.kaggle.com/datasets/dgawlik/nyse)** dataset available on Kaggle.

## **Project Objectives**

- **Data Exploration**: Perform an exploratory data analysis (EDA) to understand the dataset, including visualizations and descriptive statistics.
- **Feature Engineering and Preprocessing**: Identify and engineer relevant features, handle missing values, and transform variables for optimal model performance.
- **Model Selection and Training**: Evaluate the performance of various regression models, including Linear Regression, Lasso Regression, Ridge Regression, and XGBoost, and train them on the dataset.
- **Model Evaluation**: Assess the models' performance using the Mean Absolute Percentage Error (MAPE) metric, and compare the results.
- **Conclusion**: Summarize the findings and provide recommendations for more accurate estimation of shares outstanding.

## **Data**

The dataset used in this project is sourced from the **[New York Stock Exchange (S&P 500 companies historical prices with fundamental data)](https://www.kaggle.com/datasets/dgawlik/nyse)** dataset on Kaggle. It includes daily prices, company descriptions, and metrics extracted from annual SEC 10K fillings (2012-2016).

This analysis is focused solely on the **`fundamentals.csv`** file, which contains metrics extracted from SEC 10K fillings.

## **Contents of the Repository**

```kotlin
kotlinCopy code
.
├── README.md
├── data
│   └── fundamentals.csv
├── notebooks
│   └── Shares_Outstanding_Prediction.ipynb
├── requirements.txt
└── results
    ├── model-preformance-comparison.png
    └── true-vs-predicted-values.png

```

- **`README.md`**: Provides an overview of the project, including objectives, data sources, repository contents, and instructions for getting started.
- **`data/`**: Contains the dataset used for the analysis.
    - **`fundamentals.csv`**: Metrics extracted from SEC 10K fillings.
- **`notebooks/`**: Contains the Jupyter notebooks with the full analysis and code.
    - **`Shares_Outstanding_Prediction.ipynb`**: Jupyter notebook containing the analysis code.
- **`requirements.txt`**: Lists the required Python packages for the analysis.
- **`results/`**: Contains the results of the analysis, including model performance metrics and visualizations.
    - **`model-preformance-comparison.png`**: Visualization comparing the performance of different regression models.
    - **`true-vs-predicted-values.png`**: Visualization showing the true vs. predicted values for the best-performing model.

## **Getting Started**

1. Clone this repository to your local machine:

    ```bash
    
    git clone https://github.com/VLTSankalpa/stock-market-data-analysis.git
    cd stock-market-data-analysis
    
    ```

2. Create a virtual environment using Conda and install the required packages from **`requirements.txt`**:

    ```bash
    
    conda create -n stock_analysis python=3.8
    conda activate stock_analysis
    pip install -r requirements.txt
    
    ```

3. Open the Jupyter notebook in the **`notebooks/`** directory to start the analysis:

    ```bash
    
    jupyter notebook notebooks/Shares_Outstanding_Prediction.ipynb
    
    ```


## **Contributing**

If you have any suggestions or would like to contribute to this project, feel free to submit an issue or create a pull request.