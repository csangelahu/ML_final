# ML_final


## Set up

To set it up use conda and run

```
conda env create -f mlfinal.yaml
conda activate mlfinal
```
This will create the mlfinal environment

## Data
Original data was taken from 
- betting data: https://www.kaggle.com/datasets/visualize25/basketball-betting-dataset
- scores: https://github.com/dataquestio/project-walkthroughs/tree/master/nba_games

final_dataset.csv has the initial merged dataset. 

averages.csv and betting.csv contain the data after running preprocess.ipynb and prepare.ipynb and contains the betting information and the season long rolling averages for a team and its opponent up to a given match. Because averages.csv and betting.csv are already in the repo, you can directly run the files that train the model. 


## Running

We have 7 files 
- `preprocess.ipynb`: preprocesses data from multiple sources
- `prepare.ipynb` - creates temporal averaging features from previous stage
- `predict.ipynb` - trains the logistic regression model, does feature selection and paramater grid search for it
- `predict_dt.ipynb` - trains the decision tree model, does feature selection and paramater grid search for it
- `predict_rf.ipynb` - trains the random forest model, does feature selection and paramater grid search for it
- `predict_nn.ipynb` - trains the multilayer perception classifier model, does feature selection and paramater grid search for it
- `predict_svm.ipynb` - trains the support vector machine model, does feature selection and paramater grid search for it


