# Car Evaluation Classification

This project explores whether a car is likely to be rated as acceptable based on six characteristics: buying price, maintenance cost, number of doors, passenger capacity, luggage space, and safety. It uses the UCI Car Evaluation dataset to demonstrate how categorical data can be explored and used to train and evaluate classification models.

## Who this is for

The notebooks are intended for students, collaborators, and curious readers who want a practical introduction to data analysis and machine learning. You do not need prior knowledge of cars or machine learning to follow the analysis, but basic familiarity with Python notebooks is helpful.

## Project files

- `Project2.ipynb` explores the original four car-rating categories and compares classification approaches, including decision trees and random forests.
- `Project2_binary.ipynb` turns the ratings into two groups—unacceptable and acceptable or better—and explores classification, feature removal, and model tuning.
- `car.data`, `car.names`, and `car.c45-names` are dataset-related files included in the repository. The notebooks currently retrieve the dataset from the UCI repository when run.

## How to use it

1. Install Python 3 and JupyterLab. In a terminal, install the notebook dependencies:

   ```bash
   python -m pip install jupyterlab pandas matplotlib seaborn scikit-learn ucimlrepo
   ```

2. Download or clone this repository, then open a terminal in the project folder.
3. Start JupyterLab:

   ```bash
   jupyter lab
   ```

4. Open either notebook in the browser tab that JupyterLab opens. Use **Run → Run All Cells** to run the analysis from beginning to end.

The notebooks use `ucimlrepo` to fetch dataset 19 from the UCI Machine Learning Repository, so an internet connection is required when running them. They show data summaries and visualizations, prepare the categorical inputs for modeling, and evaluate models with held-out data and cross-validation. The binary notebook also tunes a decision tree and compares it with a random forest.

## Dataset

The dataset is the [UCI Car Evaluation dataset](https://archive.ics.uci.edu/dataset/19/car+evaluation). Its ratings come from a decision model; they should not be interpreted as evaluations of real-world vehicle performance or as evidence of causal relationships.
