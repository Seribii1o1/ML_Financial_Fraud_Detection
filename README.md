# ML_Financial_Fraud_Detection Dataset - Basic Pipeline

**Background:**

Throughout our exploration of various supervised learning algorithms, a common theme that you all might have detected (no pun intended) is the concept of extracting some signal from a noisy dataset. 
This often applies to datasets where our class of interest (fraud, basketball upset, etc) is in the “minority” class of an imbalanced dataset. 
This problem often occurs in the detection of financial fraud. While we can assume that most transactions are credible, classifying every new sample as non-fraudulent (0) will miss every single fraudulent case. 
Within this project, we will take a look at a synthetic dataset of bank transactions to see which strategies we can take in order to successfully capture as many fraudulent transactions as possible, while also minimizing false positives.

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

○ After creating the pre-processed dataset, I created a notebook where we will create train test splits and implement a RandomForestClassifier or a GradientBoostingClassifier (the choice is yours!) 
○ After training this initial classifier and viewing its accuracy measures, we will then move forward with hyperparameter tuning via GridSearchCV or 
RandomizedSearchCV (again, the choice is yours!) 
○ Upon finding optimal hyperparameters, we should re-train our model using these hyperparameters, generate predictions for this new model, and output the subsequent F1 score for this classifier.

4. Report 
○ I answered the following five project conclusion questions in report file: 
i. Which insights did you gain from your EDA? 
ii. How did you determine which columns to drop or keep? If your EDA informed this process, explain which insights you used to determine which columns were not needed. 
iii. Which hyperparameter tuning strategy did you use? Grid-search or random-search? Why? 
iv. How did your model's performance change after discovering optimal hyperparameters? 
v. What was your final F1 Score? 

1. we recommend that you look back to your previous TLABS and in-class labs. 
Looking back to our first TLAB (Rental Price Prediction), it looks like we have some template code for at least our EDA.
2. How am I supposed to run my analysis if I don’t include my dataset in GitHub? 
Keep in mind that just because something is not pushed to GItHub, does not mean that you will not be able to use it on your local machine (even if it is in your cloned git repository!) 
3. I don’t know how to make a RandomForest/GradientBoosting model. Where do I look to find this out? 
We provide links to both models. Check out the example code to get started. Also we recommend that you use Google to see how other data scientists implement these learning algorithms. 
4. How do I implement hyperparameter tuning? 
We provide links to both Grid & RandomizedSearch objects. Check out the example code provided, as well as your code from the previous weeks labs for ideas. 
5. Which model/hyperparameter tuning strategy do I choose? 
This is your executive decision to make. Better yet, why don’t you try out both and see which one performs better?
