# lazypredict

This Model help to Predict the Accuracy, Balanced Accuracy , ROC AUC , F1 Score of all ML Algorithm 

I try this model on breast cancer dataset to check the most suitable model for the this dataset 

To use this model:

Step 1 :  pip install lazypredict

Step 2 :  import lazypredict
          from lazypredict.Supervised import LazyClassifier
          from sklearn.datasets import load_breast_cancer
          from sklearn.model_selection import train_test_split

Step 3 :  data = load_breast_cancer()

Step 4 :  X = data.data
          y = data.target

Step 5 :  X_train, X_test, y_train, y_test = train_test_split(X, y,test_size=.5, random_state =12)

Step 6 : clf = LazyClassifier(verbose=0, ignore_warnings=True, custom_metric = None)

Step 7 : models,predictions = clf.fit(X_train, X_test, y_train, y_test)
         print(models)
