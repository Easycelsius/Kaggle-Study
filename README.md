# Env. Setting

```
$ source .venv/bin/activate
$ pip install kaggle
```

In kaggle site
1. Kaggle Login
2. Click the Setting
3. Create New Token
4. Download the "kaggle.json"
5. copy the file to ~/.kaggle in Linux System

# Competition Participation (Ex. Tatanic)

## Get Dataset
```
$ kaggle competitions download -c titanic
```
You can download competition dataset by Kaggle API. 
Then, you can check the titanic.zip, which has the train.csv, test.csv, and gender_submission.csv

## Create Predictive Model
- Trainig Data: train.csv
- Predicting: test.csv
- Save the result at submission.csv
- And submit to Kaggle

## Submit
```
$ kaggle competitions submit -c titanic -f gender_submission.csv -m "Submission test (gender_submission.csv)"
```

kaggle competitions submit: submit command
-c titanic: competition name
-f gender_submission.csv: result
-m "Submission test (gender_submission.csv)": description

# Reference
- https://dojang.io/mod/page/view.php?id=2470

