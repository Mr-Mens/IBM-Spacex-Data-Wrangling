# SpaceX Falcon 9 First Stage Landing Prediction: Data Wrangling Lab

## Overview

This repository provides the necessary tools and instructions for conducting exploratory data analysis (EDA) on the SpaceX Falcon 9 launch dataset. The objective is to understand the factors influencing the first stage landing success and prepare the data for predictive modeling.

## Repository Contents

- `README.md` - Instructions and information on conducting the lab exercises.
- `data_wrangling.py` - Python script for data cleaning and preparation.
- `requirements.txt` - List of Python packages required to run the scripts.

## Prerequisites

Ensure you have Python installed on your computer (Python 3.8+ recommended). Additionally, install the necessary Python libraries using:

```bash
pip install -r requirements.txt
```

## Lab Objective

The goal of this lab is to perform data wrangling to set up a clean dataset for subsequent analysis. Specifically, you will convert raw launch outcome data into a format suitable for training machine learning models.

### Estimated Time to Complete: 60 minutes

## Instructions

### Step 1: Set Up Your Environment

Clone the repository and navigate into the project directory:

```bash
git clone https://github.com/your-username/spacex-data-wrangling-lab.git
cd spacex-data-wrangling-lab
pip install -r requirements.txt
```

### Step 2: Data Wrangling

Run the `data_wrangling.py` script to start the data cleaning process:

```bash
python data_wrangling.py
```

This script performs the following operations:

- Loads the dataset from a CSV file.
- Identifies and handles missing values.
- Converts launch outcomes into binary labels for classification (1 for success, 0 for failure).
- Saves the cleaned data to a new CSV file.

### Step 3: Explore the Cleaned Data

After cleaning the data, explore the dataset to understand its structure and contents:

```python
import pandas as pd
data = pd.read_csv('dataset_part_2.csv')
print(data.head())
```

## Task Highlights

1. **Exploratory Data Analysis (EDA)**: Identify patterns and missing values in the dataset.
2. **Label Determination**: Convert textual launch outcomes into binary labels suitable for supervised learning.
3. **Data Cleaning**: Address missing and inconsistent data entries.

## Expected Outputs

The `data_wrangling.py` script will output a CSV file named `dataset_part_2.csv`, which will contain the cleaned and preprocessed launch data including binary labels for the landing outcome.

## Data Fields

- **Launch Site**: The site from which the Falcon 9 was launched.
- **Orbit**: The orbit type targeted for the mission.
- **Payload Mass**: The mass of the payload carried by Falcon 9.
- **Outcome**: Textual description of the launch outcome.
- **Class**: Binary label indicating the success (1) or failure (0) of the landing.

## Authors

- [Joseph Santarcangelo](https://www.linkedin.com/in/joseph-s-50398b136/) - PhD in Electrical Engineering, specializes in using machine learning for video analytics. Currently a Data Scientist at IBM.
- [Nayef Abou Tayoun](https://www.linkedin.com/in/nayefaboutayoun/) - Data Scientist at IBM, pursuing a Master’s degree in Artificial Intelligence at Queen's University.

## Change Log

| Date (YYYY-MM-DD) | Version | Changed By      | Change Description                 |
|-------------------|---------|-----------------|------------------------------------|
| 2021-08-31        | 1.1     | Lakshmi Holla   | Updated markdown formatting        |
| 2021-05-26        | 1.1     | Joseph          | Updated input data and instructions|
| 2020-11-04        | 1.1     | Nayef           | Updated input data format          |
| 2020-09-20        | 1.0     | Joseph          | Created initial version of the lab |

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE.md) file for details.

Contributions, forks, and feedback are welcome to improve this lab and make the data wrangling process more comprehensive and accessible.
