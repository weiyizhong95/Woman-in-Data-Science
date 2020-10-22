# Woman-in-Data-Science


Introduction¶
In this project, we will be using patient health data from MIT's GOSSIS(Global Open Source Severity of Illness Score) to do an experiment, in which we want to evaluate the question of which modeling strategy leads to the most effective predictions. The training dataset contains 91713 entries and 186 variables including age, gender, height etc. There are 5 models chosen, KNN, Logsitic Regression, Random Forest, Boosting Models, and Neural Networks.For one model approach, we are training and testing on the whole dataset. For the many model approach, we are training and testing the model on 5 age subgroups of dataset. The goal is to test which approach performs better.

There are in toal 5 parts in this project, data preprocessing, Adversarial Validation, data modeling(One-Model approach, Many-Model approach), scoreboard, disscusion and references. 

In the data preprocessing part, first, I decide to delete varibles having no or very few repeated values. Second, the percentage of missing values higher than 80%. After that, I check the missing values in train and test data, categorical and numeri variables separately, and fill the NAs according to the pattern, with the first type of categorical variable, or adding a type of 'missing', or 0, or median, or random, or mean. 

In the Adversarial validation part, I use the cleaned data obtained from above process, and predict the results with random forest, which returns a roc_auc of nearly 50%.

Then in the data modeling parts, models used are listed above. Scores are listed in the scoreboard. Discussion is about my findings during the whole process. At last is the references.
