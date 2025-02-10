# King County House Price Prediction

This repository hosts a Jupyter notebook dedicated to predicting house prices in King County, using regression analysis, enriched by web-scraped demographic data, and extensive feature engineering techniques.

## Project Overview

The goal of this project is to predict house prices in King County by employing regression models and enhancing the dataset with additional city-level information obtained through web scraping. The analysis integrates sophisticated feature selection and evaluation methods to build a predictive model that can estimate house prices based on various property characteristics and demographic insights.

## Features

- **Web Scraping**: Automated collection of city and population data for each zipcode to enrich the dataset.
- **Data Preprocessing**: Standardization and cleaning of data to prepare for analysis.
- **Feature Selection Techniques**:
  - `SelectKBest` with `mutual_info_regression` and `f_regression` to identify significant features.
  - **Feature Ranking**: Utilization of `ExtraTreesRegressor` and `RandomForestRegressor` for ranking features based on their importance.
- **City Level Analysis**:
  - Computation of average house prices and population by city to provide contextual insights.
- **Regression Models**: Application of various regression techniques to forecast house prices.
- **Model Evaluation**:
  - Use of a pipeline approach to streamline preprocessing and model evaluation.
  - Performance metrics such as RMSE (Root Mean Square Error) and R-squared to assess model accuracy.

## Methodology

1. **Data Collection**:
   - Utilize the King County House Sales dataset from public sources.
   - Web scrape additional demographic data related to city populations and features for each zipcode.

2. **Data Preprocessing**:
   - Clean and normalize the data, ensuring it is suitable for the analysis.

3. **Feature Engineering**:
   - Implement `SelectKBest` for feature selection to enhance model performance.
   - Rank features using tree-based models to identify the most predictive features.

4. **City Level Analysis**:
   - Analyze average prices and population metrics by city to provide deeper market insights.

5. **Modeling**:
   - Configure pipelines for regression models including linear regression and ensemble methods.
   - Train and evaluate models using cross-validation.

6. **Evaluation**:
   - Detailed analysis of model performance using statistical metrics.

## Future Work

- Integrate more advanced machine learning models to improve prediction accuracy.
- Expand the dataset with additional features such as economic indicators and more detailed property characteristics.
- Apply the modeling framework to other geographic locations for broader real estate market analysis.

## Contributing

Contributions are welcome! You can contribute by:
- Enhancing model accuracy and efficiency.
- Expanding the dataset with new features.
- Improving the feature selection and engineering processes.

Please open an issue to discuss significant changes before making a pull.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.
