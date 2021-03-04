# Research Paper classification


_When going through the data, I noticed that the training dataset had its target variables/labels missing, Hence I created a new .csv file called '**result.csv'**.
_


**OBSERVATIONS**:

1. The data was already divided into training and testing data, with training data having both the dependent and independent variables, whilst the training data set had no target variables
2. The target variables were encoded in the "One-hot encoding" format with observations having both single and multiple tags, which qualifies it for multilabel classification 
3. The corpus first had stop words removed from it and later punctions too
4. stemming and lematization further removed the unecessary prefixes
5. Machines do not understand numerical data so the corpus was vectorized using TF IDF where the "importance" or weight is calcualted as 
Weight = log(1+TF) * (N/df) to represent them in a space where their distance from each other should correspond to their similarity semantically.
5. Modelling the data is the next step, After fitting the data, I realized that the evaluation of multi label classification was not as easy as regular binary classification, A confusion matrix was plotted
6. The tesing data was used as out of sample data to predict values and they were saved in "result.csv"
