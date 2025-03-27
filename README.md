# ML_Financial_Fraud_Detection Dataset - Basic Pipeline

**Background:**

Throughout our exploration of various supervised learning algorithms, a common theme is the concept of extracting some signal from a noisy dataset. 
This often applies to datasets where our class of interest (fraud, basketball upset, etc) is in the “minority” class of an imbalanced dataset. 
This problem often occurs in the detection of financial fraud. While we can assume that most transactions are credible, classifying every new sample as non-fraudulent (0) will miss every single fraudulent case. 
Within this project, I look at a synthetic dataset of bank transactions to see which strategies I can take in order to successfully capture as many fraudulent transactions as possible, while also minimizing false positives.

I created a comprehensive machine-learning pipeline that satisfies the patterned steps of a classic machine learning project:

● hypothesis formulation through EDA

● data cleaning & pre-processing 

● model generation and a report

**Project Description**

Notebooks: 
1. Initial EDA 

○ Project begins with a notebook with univariate, bivariate, multivariate exploratory analysis, and relevant graphs.

2. Data cleaning, wrangling & pre-processing

○ After completing EDA, I created a notebook to clean and wrangle the dataset. This might include dropping null values, removing unnecessary columns, removing outliers, and potentially fixing incorrectly formatted data.

○ I saved this dataframe as a new csv file to be used in the next step.

3. Model creation, hyperparameter search, and model evaluation 

○ After creating the pre-processed dataset, I created a notebook where I created train test splits and implemented numerous classifiers

○ After training the initial classifiers and viewing their accuracy measures, I used hyperparameter tuning (GridSearchCV, 
RandomizedSearchCV)

○ Upon finding optimal hyperparameters, I re-trained the models using these hyperparameters, generate predictions for this new model, and output the subsequent F1 scores for the classifiers

4. Report 

○ I answered the following five project conclusion questions in report file: 
i. Which insights did you gain from your EDA? 
ii. How did you determine which columns to drop or keep? If your EDA informed this process, explain which insights you used to determine which columns were not needed. 
iii. Which hyperparameter tuning strategy did you use? Grid-search or random-search? Why? 
iv. How did your model's performance change after discovering optimal hyperparameters? 
v. What was your final F1 Score? 


