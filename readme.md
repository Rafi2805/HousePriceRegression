# House Price Regression Project
[Website Project Description](https://www.kaggle.com/competitions/ifsul-clube-de-ia-house-prices-regression/overview)

## Setup

### create virtual environment

```zsh
# cd into project folder

python3 -m venv venv

source venv/bin/activate

pip install kaggle

```

## First Example

[Solution for Beginners](https://www.kaggle.com/code/akhileshthite/house-prices-solution-for-beginners)

- as seen in the example.py file
- i made it close to the original but with some modifications for scripting and not a notebook


## Ideas

- dataset cleaning only needs to be done once
  - set up script to clean up our datasets and re-export them
    - model selection is the iterative process so get a modeling script up to start this process

### Possibilities

#### Currently Implemented
- Random Forest
- Gradient Boosting Machines (GBM)

#### Todo
- Linear Regression
- Decision Trees
- Support Vector Regressor (SVR)
- Neural Networks
- XGBoost, LightGBM, etc.



### Start

I have preprocessed housing data split into training and testing sets (X_train, X_test, y_train, y_test).
Python script that will:

Train multiple regression models (e.g., Linear Regression, Random Forest, Gradient Boosting, XGBoost, and Neural Networks).
Evaluate their performance using common metrics like Root Mean Squared Error (RMSE) or R² score.
Include hyperparameter tuning for models using GridSearchCV or RandomizedSearchCV.
Rank models based on performance and output the model with the best score.
Optionally, visualize model performance using a bar chart.
Provide options to save the trained models and predictions.



## Work Flow
- Use features / feature_extraction to investigate which features are most important for training
- create a copy of model_template and name with method type
- rename function inside of model_template and setup testing scripts inside __main__




## Lab Server

```zsh
ssh kmcknze1@c2-kevin.uom.memphis.edu
```
```zsh
cd HousePriceRegression
tmux # allows you leave while it's running
source venv/bin/activate
git pull # if necessary
python3 -m models.gradient_boosting_GS # or whatever model
```
- to exit and let it keep running
- press ctr+b
- press d (for detach)
- now you can leave and it'll keep running
- to go back in and check on it

```zsh
tmux attach
```