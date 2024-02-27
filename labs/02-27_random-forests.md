# Random Forests

A major theme in data science is continuous learning. There are often times where you'll need to use a model form you're unfamiliar with, or even to immplement one from scratch based on academic research.

For this lab, the goal is to understand, implement, and validate a random forest model in Python.

## The Task

Build a random forest model to predict housing prices using the following California house price dataset:

```python
train_df = pd.read_csv("https://download.mlcc.google.com/mledu-datasets/california_housing_train.csv")
train_df = train_df.reindex(np.random.permutation(train_df.index))

test_df = pd.read_csv("https://download.mlcc.google.com/mledu-datasets/california_housing_test.csv")
```

## The Deliverables

At the end of this lab, you should submit (in the form of a Jupyter notebook):

  - A written narrative explaining what a random forest is, and at a high level how it "learns", targeted at a non-technical audience;
  - A minimal data processing (cleaning and feature engineering) pipeline;
  - A written plan of analysis: what's the outcome you're predicting, how are you predicting it, and why did you land on that strategy;
  - A trained random forest / gradient boosted tree model;
  - A narrative evaluation of your model's performance
