# What

This project goal is to predict student's performance based on their socio-economic status and other factors. The data comes from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/320/student+performance).

The data contains features such as:
- students' previous school,
- parents' education,
- parents' occupation,
- students' internet access

and many more.

The data set three different targets - students' scores at the end of
- first grade (G1), 
- second grade (G2),
- third grade (G3). 

To simplify the model, we will only use the G1 early on. We'll see what accuracy we can achieve with the given features and models. Since G1-G3 are given in a scale of 1-20, we'll simplify the problem to a binary one, only predicting whether the student will pass or fail.

Later on, we'll move G1 and G2 to features and predict G3, to see how does student's recent performance in the same school affect their future performance.

We'll use two models here:
- AdaBoost with Decision Tree Classifier
- Keras Sequential Model

and compare their performance.

# How

To run the project, install the dependencies using `requirements.txt` file:

```bash
pip install -r requirements.txt
```

Then, open the `model.ipynb` file and run the cells one by one.

For your convenience, there are `G1` and `G3_with_G1_G2` random search results directiores. Thanks to them you can skip rather lengthy hyperparameter search. If you want to re-run the search, just remove those files and run the cells again.