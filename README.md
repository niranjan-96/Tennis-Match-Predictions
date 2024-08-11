# Tennis Match Outcome Prediction Models

This repository is dedicated to predicting the outcomes of ATP tennis matches using sophisticated probabilistic models. By leveraging a rich dataset of tennis match records from 2005 to 2018, various models have been developed and trained to forecast match results for the 2019 season. The project explores and compares several predictive approaches, including a Naive model, Univariate Logistic Regression, Elo-based models, and the Bookmakers Consensus Model (BCM). Additionally, the models are enhanced with surface-specific adjustments to improve prediction accuracy.

## Project Overview

The primary goal of this project is to build and evaluate models that can accurately predict the outcomes of professional men's tennis matches. By analyzing historical data, the models aim to identify patterns and factors that influence match results. The focus is on ensuring that the models generalize well to unseen data, particularly the match outcomes from 2019.

### Models Implemented:
- **Naive Model**: A simple baseline model based on basic assumptions.
- **Univariate Logistic Regression Model**: A model that predicts match outcomes using logistic regression on a single feature.
- **Elo-based Models**: Variations of the Elo rating system, including standard, surface-specific, and margin of victory (MOV) enhancements.
- **Bookmakers Consensus Model (BCM)**: A model that incorporates betting odds to predict match outcomes.

## Dataset

### Source:
The dataset used in this project is sourced from [tennis-data.co.uk](http://www.tennis-data.co.uk/).

### Description:
The dataset consists of comprehensive records of ATP men's professional tennis matches, covering the period from 2005 to 2018. It includes detailed information such as player rankings, match results, court surfaces, and betting odds. This historical data is utilized to train the models, while match data from 2019 is reserved for validation and testing purposes.

## Repository Structure

### Folders:
- **dataset**: Contains the dataset files needed to train and validate the models.
- **Code**: Includes all Jupyter notebooks implementing the various prediction models.

### Key Files:
- **BCM_Model.ipynb**: Implements the Bookmakers Consensus Model (BCM).
- **ELO_538_Model.ipynb**: Features the Elo rating model based on FiveThirtyEight's methodology.
- **ELO_538_Model_Surface_Specific.ipynb**: A variation of the Elo model with adjustments for different court surfaces.
- **ELO_K_factor_Model.ipynb**: Implements the classic Elo rating system with a fixed K-factor.
- **ELO_K_Factor_Model_Surface_Specific.ipynb**: A surface-specific version of the Elo K-factor model.
- **ELO_Linear_MOV_Model.ipynb**: Extends the Elo model by incorporating a linear margin of victory (MOV) component.
- **ELO_Linear_MOV_Model_Surface_Specific.ipynb**: A surface-adjusted version of the Linear MOV model.
- **Logistic_Regression_Model.ipynb**: Implements logistic regression to predict match outcomes.
- **Naive_Model.ipynb**: A simple model serving as a baseline for comparison.

## Usage

1. **Data Preparation**: Place the dataset files in the `dataset` folder.
2. **Running Models**: Navigate to the `Code` folder and open the desired Jupyter notebook. Follow the steps in the notebook to train and evaluate the models.
3. **Parameter Tuning**: Some notebooks allow tuning of hyperparameters such as `K` and `sigma` to optimize model performance.
4. **Visualization**: The notebooks include plots to visualize results and help in analyzing model performance.

## Results and Analysis

The models are evaluated on their ability to predict the outcomes of 2019 ATP matches. Key performance metrics include log-loss, accuracy, and calibration. The results help identify the most effective models and parameter settings.

## Contact

For questions or suggestions, please open an issue or reach out to the repository owner.
