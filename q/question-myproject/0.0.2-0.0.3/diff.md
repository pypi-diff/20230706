# Comparing `tmp/question-myproject-0.0.2.tar.gz` & `tmp/question-myproject-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "question-myproject-0.0.2.tar", last modified: Wed Jul  5 22:16:36 2023, max compression
+gzip compressed data, was "question-myproject-0.0.3.tar", last modified: Thu Jul  6 14:29:47 2023, max compression
```

## Comparing `question-myproject-0.0.2.tar` & `question-myproject-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 22:16:36.547949 question-myproject-0.0.2/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-07-05 21:49:48.000000 question-myproject-0.0.2/LICENSE
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      494 2023-07-05 22:16:36.547949 question-myproject-0.0.2/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      117 2023-07-05 21:55:22.000000 question-myproject-0.0.2/pyproject.toml
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      620 2023-07-05 22:16:36.547949 question-myproject-0.0.2/setup.cfg
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 22:16:36.543949 question-myproject-0.0.2/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 22:16:36.543949 question-myproject-0.0.2/src/generator/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-07-05 22:06:50.000000 question-myproject-0.0.2/src/generator/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4292 2023-07-05 22:15:15.000000 question-myproject-0.0.2/src/generator/main.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-05 22:16:36.547949 question-myproject-0.0.2/src/question_myproject.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      494 2023-07-05 22:16:36.000000 question-myproject-0.0.2/src/question_myproject.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      264 2023-07-05 22:16:36.000000 question-myproject-0.0.2/src/question_myproject.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-07-05 22:16:36.000000 question-myproject-0.0.2/src/question_myproject.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       10 2023-07-05 22:16:36.000000 question-myproject-0.0.2/src/question_myproject.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-06 14:29:47.395009 question-myproject-0.0.3/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-07-05 21:49:48.000000 question-myproject-0.0.3/LICENSE
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      494 2023-07-06 14:29:47.395009 question-myproject-0.0.3/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      117 2023-07-05 21:55:22.000000 question-myproject-0.0.3/pyproject.toml
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      620 2023-07-06 14:29:47.395009 question-myproject-0.0.3/setup.cfg
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-06 14:29:47.391009 question-myproject-0.0.3/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-06 14:29:47.395009 question-myproject-0.0.3/src/generator/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-07-05 22:06:50.000000 question-myproject-0.0.3/src/generator/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4567 2023-07-06 14:28:43.000000 question-myproject-0.0.3/src/generator/main.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-07-06 14:29:47.395009 question-myproject-0.0.3/src/question_myproject.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      494 2023-07-06 14:29:47.000000 question-myproject-0.0.3/src/question_myproject.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      264 2023-07-06 14:29:47.000000 question-myproject-0.0.3/src/question_myproject.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-07-06 14:29:47.000000 question-myproject-0.0.3/src/question_myproject.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       10 2023-07-06 14:29:47.000000 question-myproject-0.0.3/src/question_myproject.egg-info/top_level.txt
```

### Comparing `question-myproject-0.0.2/setup.cfg` & `question-myproject-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = question-myproject
-version = 0.0.2
+version = 0.0.3
 author = Patrick
 author_email = Patrick@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `question-myproject-0.0.2/src/generator/main.py` & `question-myproject-0.0.3/src/generator/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,56 +7,67 @@
 from sklearn.datasets import make_classification, make_regression
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import mean_squared_error, accuracy_score
 from sklearn.metrics import confusion_matrix
 
+
 def generate(problem, n_samples, n_features):
     """
     Generate a dataset
     """
     if problem == "classification":
-        print("Generate a classification dataset with {} samples, {} features and 2 classes".format(n_samples, n_features))
-        X, y = make_classification(n_samples=n_samples, n_features=n_features, n_classes=2)
+        print("Generate a classification dataset with {} samples, {} features and 2 classes".format(
+            n_samples, n_features))
+        X, y = make_classification(
+            n_samples=n_samples, n_features=n_features, n_classes=2)
 
     elif problem == "regression" or problem == "ordinaryleastsquaresregression":
-        print("Generate a regression dataset with {} samples and {} features".format(n_samples, n_features))
-        X, y = make_regression(n_samples=n_samples, n_features=n_features, noise=10)
+        print("Generate a regression dataset with {} samples and {} features".format(
+            n_samples, n_features))
+        X, y = make_regression(n_samples=n_samples,
+                               n_features=n_features, noise=10)
 
     else:
         raise Exception("Unknown problem")
 
     return X, y
 
+
 def get_metric(problem):
     """
     Get the metric for computing the model performances
     """
     if problem == "classification":
         return accuracy_score
 
     elif problem == "regression" or problem == "ordinaryleastsquaresregression":
         return mean_squared_error
 
     else:
         raise Exception("Unknown problem")
 
+
 def learn(problem, X, y):
     """
     Learn a linear model
     """
     if problem == "classification":
         print("Learning a Linear Discriminant Analysis.", end=" ")
         model = LinearDiscriminantAnalysis()
 
     elif problem == "regression":
         print("Learning a Linear Regression.", end=" ")
         model = LinearRegression()
 
+    elif problem == "ordinaryleastsquaresregression":
+        print("Learning an Ordinary Linear Regression.", end=" ")
+        model = LinearRegression()
+
     else:
         raise Exception("Unknown problem")
 
     # Train/test splitting
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=.33)
 
     # Model fitting
@@ -69,14 +80,15 @@
 
     if problem == "classification":
         print("Confusion matrix:")
         print(confusion_matrix(y_test, y_pred))
 
     return model, error
 
+
 def predict(model, problem):
     """
     Predict new date
     """
     # Generate a new dataset
     print("Predict on a new dataset of 10 values")
     try:
@@ -84,45 +96,53 @@
     except AttributeError:
         coefs = model.coefs_.ravel()
     X, _ = generate(problem, 10, len(coefs))
 
     # Call the model
     return model.predict(X)
 
+
 def target_statistics(y):
     """
     Stats for the target vector
     """
     mean_target = np.mean(y)
     std_target = np.std(y)
-    print("Statistics of the target. Mean = {}, std = {}".format(mean_target, std_target))
+    print("Statistics of the target. Mean = {}, std = {}".format(
+        mean_target, std_target))
     return mean_target, std_target
 
+
 def features_statistics(X):
     """
     Stats for the features
     """
-    mean_features = {"feature_{}".format(k): np.mean(X[:,k]) for k in range(X.shape[1])}
+    mean_features = {"feature_{}".format(k): np.mean(
+        X[:, k]) for k in range(X.shape[1])}
     print("Mean values of the features:")
     print(json.dumps(mean_features, indent=4))
 
-    std_features = {"feature_{}".format(k): np.std(X[:,k]) for k in range(X.shape[1])}
+    std_features = {"feature_{}".format(k): np.std(
+        X[:, k]) for k in range(X.shape[1])}
     print("Std values of the features:")
     print(json.dumps(std_features, indent=4))
 
     return mean_features, std_features
 
+
 def correlation(X, y):
     """
     Pearson correlation coefficient
     """
-    corr_coefs = {"feature_{}".format(k): np.corrcoef(X[:,k], y) for k in range(X.shape[1])}
+    corr_coefs = {"feature_{}".format(k): np.corrcoef(
+        X[:, k], y) for k in range(X.shape[1])}
     print_correlations(X, y)
     return corr_coefs
 
+
 def statistics(X, y):
     """
     Compute descriptive statistics from the data
     """
     print("Compute the statistics")
     mean_target, std_target = target_statistics(y)
     mean_features, std_features = features_statistics(X)
@@ -132,14 +152,15 @@
         "mean_target": mean_target,
         "std_target": std_target,
         "mean_features": mean_features,
         "std_features": std_features,
         "correlations": corr_coefs
     }
 
+
 def print_correlations(X, y):
     """
     Print the correlation of the dataset
     """
-    dataset = np.concatenate([X, y.reshape(-1,1)], axis=1)
+    dataset = np.concatenate([X, y.reshape(-1, 1)], axis=1)
     print("Dataset correlation matrix:")
     print(np.round(np.corrcoef(dataset), 2))
```

