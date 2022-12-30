# DS-GA 3001 Final Project

In this folder we have three subfolders:

/code: the folder that contains the harness function 

/data: the folder that contains all external data that will be read in by harness function

/model: the folder that contains pre-trained CatBoost model

How to run the harness function:

```
conda create -n CDSML poetry 
conda activate CDSML 
poetry install
cd code
jupyter notebook
````

Then put the test data file into the `data` folder.

Open the `harness.ipynb` file and set the `TEST_FILENAME` variable. Run the notebook cells.

There should only be one function inside called `harness(df)`. 
The output of harness function should be a n*1 vector of predicted default probability, with n=len(df).
