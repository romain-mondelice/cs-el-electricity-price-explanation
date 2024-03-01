# CentraleSupélec & ESSEC - Esemble Learning Course - Project: Explaining Electricity Price Variations

## Abstract

This project aims to explain the daily price variation of electricity futures contracts in France and Germany using ensemble learning techniques. By analyzing weather, energy production, and electricity usage data, we seek to build models that can estimate these price variations effectively. Unlike traditional prediction problems, our focus is on understanding the factors that contribute to price fluctuations in the electricity market.

## Project Goals

1. **Model Development**: Utilize ensemble learning methods taught in the course, including Decision Trees, Bagging, Random Forests, Boosting, Gradient Boosted Trees, and AdaBoost, to build models that explain the variability in electricity price variations.
2. **Performance Comparison**: Evaluate the models using metrics like Mean Squared Error (MSE) and Mean Absolute Error (MAE) to assess their explanatory power.
3. **Report Writing**: Summarize findings and model performances in a concise report, adhering to a five-page limit.

## Dataset Description

The dataset comprises three CSV files:
- **Training Inputs (X_train)**: Features including weather conditions, energy production metrics, and electricity usage data.
- **Training Outputs (Y_train)**: Target variable representing daily price variation for 24H electricity baseload futures.
- **Test Inputs (X_test)**: Features for the test set to evaluate model performances.

Each input dataset contains 35 columns, including identifiers for days and countries, weather measures, energy production measures, and electricity use metrics. The output datasets contain identifiers and the target variable.

## Installation and Usage

1. **Clone the Repository**: `git clone [repository-link]`
2. **Install Required Libraries**: `pip install -r requirements.txt`
3. **Run the Analysis**: `python analysis_script.py`

## Benchmark

The benchmark model is a simple linear regression with minimal data cleaning. This project aims to surpass this benchmark by employing advanced ensemble learning techniques.

## Team Members

- Raphael Monges
- Romain Mondelice
- Antoine Bossan
- Hanyun Hu

## Acknowledgments

We thank CentraleSupélec and our course instructors for guiding us through the ensemble learning methods and providing us with the opportunity to work on this real-world challenge.

## Data Source

Data for this project was obtained from the ENS Data Challenge website. [Access the data here](https://challengedata.ens.fr/challenges/97).

## Project Structure

Below is the recommended project structure, enabling a modular and manageable codebase.

```
├── LICENSE            <- Information about the license of your code. Companies may have guidelines on how to license code. [See more here](https://choosealicense.com/)
├── README.md          <-  A README file for developers to understand the project setup and instructions.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   ├── presentation   <- Presentation of the project.
│   └── figures        <- Graphics and figures for use in reports.
│ 
├── requirements.txt   <- Required libraries and dependencies. 
│
├── pyproject.toml     <- Make the project pip installable with `pip install -e`.
```
