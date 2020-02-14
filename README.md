# DSCI6672
AI &amp; Cybersecurity


LAOISE LUCIANO - PHISHING MACHINE LEARNING

February 13, 2020

This was a project for my AI Cybersecurity class during the Spring 2020 Semester at the University of New Haven.

Our objective was to train a single-layer perceptron model to create a phish detector. We used the Phishing Website dataset ( https://archive.ics.uci.edu/ml/datasets/phishing+websites ) for training and evaluation of our model. The description of features can be found in the Data Folder at the following website.

To begin, the dataset available above was converted to a csv workbook and stripped of headers so that the top row would not skew results. This was imported as a dataset named TrainingDataset-noheaders.csv which can be found in this corresponding GitHub.

As the first column in the dataset was the ID of the sample, the data was selected in a data frame using column 1 as the start and ending on column 30, ignoring the final results column. The dataset was split into 4 datasets with a test size of 30% of the dataset.

Perceptron was utilized with 40 sample iterations to fit the data. In our particular dataset, a comparison of the test and prediction data resulted in a 91% accuracy with only 282 misclassified samples. In the demonstrated ROC curve, our model has an AUC or Area under the Curve of .97. The closer this number is to 1.0, the better the model is at separating distinctions between classes. Since this model has a 0.97 number with only 0.03 difference, this model is a good model for determining whether an item is a phishing website.

