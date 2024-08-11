# Tennis Match Outcome Prediction Models

This repository contains a collection of models used for predicting the outcomes of tennis matches. The models implemented here include variations of the Elo rating system, a Betting Confidence Model (BCM), logistic regression, and a naive model. The repository is organized into two main folders: `dataset` and `Code`.

## Repository Structure

### Folders:
- **dataset**: This folder contains all the datasets used for training and validating the models. Ensure that the datasets are properly formatted and preprocessed before running the models.
  
- **Code**: This folder contains all the Jupyter notebooks implementing the various prediction models. Each notebook is self-contained and can be run independently, depending on the specific model you wish to evaluate or modify.

### Files:
- **BCM_Model.ipynb**: Implements the Betting Confidence Model, which is designed to predict match outcomes based on historical betting data.
  
- **ELO_538_Model.ipynb**: This notebook implements the Elo rating system based on the FiveThirtyEight model, adapted for tennis.
  
- **ELO_538_Model_Surface_Specific.ipynb**: A variant of the Elo 538 model that takes into account the surface-specific performance of players.
  
- **ELO_K_factor_Model.ipynb**: Implements the standard Elo rating system with a constant K-factor for updating ratings.
  
- **ELO_K_Factor_Model_Surface_Specific.ipynb**: A surface-specific variant of the Elo K-factor model.
  
- **ELO_Linear_MOV_Model.ipynb**: Implements the Elo rating system incorporating a linear margin of victory (MOV) model, where rating updates depend on the margin by which matches are won.
  
- **ELO_Linear_MOV_Model_Surface_Specific.ipynb**: A surface-specific variant of the Elo Linear MOV model.
  
- **Logistic_Regression_Model.ipynb**: Implements a logistic regression model to predict match outcomes based on a range of input features.
  
- **Naive_Model.ipynb**: A simple naive model that predicts outcomes based on basic assumptions, serving as a baseline for comparison with more complex models.

## Usage

1. **Data Preparation**: Ensure that all the datasets are placed in the `dataset` folder and are correctly formatted.
  
2. **Running the Models**: Navigate to the `Code` folder and open the Jupyter notebook for the model you want to run. You can execute the cells sequentially to train and evaluate the model.

3. **Parameter Tuning**: Some notebooks include parameter grids for tuning hyperparameters (e.g., `K` and `sigma` in the Elo models). You can adjust the range of these parameters to find the best model configurations.

4. **Visualization**: The notebooks include various plots to visualize the results, such as the relationship between parameters and log-loss. Make sure to run all cells to generate the plots.

## Results

After running the models, you can analyze the performance metrics, such as log-loss, accuracy, and calibration. The best-performing models based on these metrics can be identified and used for further analysis or prediction.

## Contact

If you have any questions or suggestions, feel free to open an issue or contact the repository owner.
