The Federal Reserve's monetary policy decisions, particularly those concerning the Fed Fund rate, hold significant implications for various financial markets and economic activities. Among these, the impact on mortgage rates is particularly crucial for the average American. Therefore, this study aims to explore the relationship between changes in the Fed Fund rate and mortgage rates, specifically focusing on the 30-year mortgage rate.
# Interest Rates Analysis

This project analyzes the relationship between various interest rates and the Federal Fund rate using R. It includes linear regression models and visualizations to explore these relationships.

## Table of Contents
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis Overview](#analysis-overview)
- [Visualizations](#visualizations)

## Prerequisites

- R (version 3.0.0 or higher recommended)
- RStudio (optional, but recommended)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/your-username/interest-rates-analysis.git
   ```

2. Install required R packages:
   ```R
   install.packages(c("readxl", "ggplot2"))
   ```

## Usage

1. Place your Excel file named "cleaned data rates (3).xlsx" in the project directory.

2. Open the R script in RStudio or your preferred R environment.

3. Update the file path in the script if necessary:
   ```R
   data <- read_excel("/path/to/your/cleaned data rates (3).xlsx", sheet = 1)
   ```

4. Run the script to perform the analysis and generate visualizations.

## Analysis Overview

The script performs the following analyses:

1. Data Loading and Preparation:
   - Loads data from an Excel file
   - Converts date column to proper Date type
   - Adds a sequential order variable

2. Linear Regression Models:
   Four models are fitted, comparing each of these rates to the Federal Fund rate:
   - 1-year Treasury rate
   - 10-year Treasury rate
   - 30-year Treasury rate
   - 30-year mortgage rate

3. Model Summaries:
   For each model, a summary is provided including:
   - Coefficients (intercept and slope)
   - Standard errors
   - T-values and p-values
   - R-squared values
   - F-statistic and its p-value

## Visualizations

The script generates four scatter plots using ggplot2:

1. 1-year Treasury rate vs. Fed Fund rate
2. 10-year Treasury rate vs. Fed Fund rate
3. 30-year Treasury rate vs. Fed Fund rate
4. 30-year mortgage rate vs. Fed Fund rate

These visualizations help to illustrate the relationship between each interest rate and the Federal Fund rate.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
