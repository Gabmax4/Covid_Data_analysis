# Covid Data Analysis

This project performs a full exploratory data analysis of global COVID-19 data, with a special focus on Latin American countries. It uses data from Johns Hopkins University and various Python libraries for data manipulation and visualization.

## 1.0 Full Exploratory Data Analysis

### 1.1 Libraries

The project uses the following libraries:

- `pandas`: For data manipulation.
- `matplotlib`: For data visualization.
- `seaborn`: For data visualization.
- `janitor`: For data cleaning and transformation.
- `final_project.utils.paths`: For file path management.

### 1.2 Download Data

The data is downloaded from the Johns Hopkins University repository:

- URL: `https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_global.csv`

### 1.3 Process Data

The data is processed to convert it into a format suitable for analysis:

- Relevant columns are selected.
- The data structure is transformed to facilitate temporal analysis.
- Column names are cleaned.

### 1.4 Explore Data

Several visualizations are created to explore the data:

- Time series of COVID-19 cases in Latin American countries.
- Comparison of Latin American countries in the global context.

### 1.5 Save Processed Data

The processed data is saved to a CSV file for further analysis.
  
## Installation guide

Please read [install.md](install.md) for details on how to set up this project.

## Project Organization

    ├── LICENSE
    ├── tasks.py           <- Invoke with commands like `notebook`.
    ├── README.md          <- The top-level README for developers using this project.
    ├── install.md         <- Detailed instructions to set up this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures         <- Generated graphics and figures to be used in reporting.
    │
    ├── environment.yml    <- The requirements file for reproducing the analysis environment.
    │
    ├── .here              <- File that will stop the search if none of the other criteria
    │                         apply when searching head of project.
    │
    ├── setup.py           <- Makes project pip installable (pip install -e .)
    │                         so final_project can be imported.
    │
    └── final_project               <- Source code for use in this project.
        ├── __init__.py    <- Makes final_project a Python module.
        │
        ├── data           <- Scripts to download or generate data.
        │   └── make_dataset.py
        │
        ├── features       <- Scripts to turn raw data into features for modeling.
        │   └── build_features.py
        │
        ├── models         <- Scripts to train models and then use trained models to make
        │   │                 predictions.
        │   ├── predict_model.py
        │   └── train_model.py
        │
        ├── utils          <- Scripts to help with common tasks.
            └── paths.py   <- Helper functions to relative file referencing across project.
        │
        └── visualization  <- Scripts to create exploratory and results oriented visualizations.
            └── visualize.py


# How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Gabmax4/Covid_Data_analysis.git
   cd Covid_Data_analysis
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the exploratory data analysis notebook:
   ```bash
   jupyter notebook notebooks/exploratory_data_analysis.ipynb
   ```
---
Project based on the [cookiecutter conda data science project template](https://github.com/jvelezmagic/cookiecutter-conda-data-science).# Covid_Data_analysis
