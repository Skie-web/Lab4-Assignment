# Lab4-Assignment

Student number 230793983
BICT 332 Artficial Intelligence
Lab Asignment 4

In the lab what was learned is to preprocess data by handling missing values(drop/impute), encoding categories (mapping/ one-hot), split datasets (stratified), scale features (norm/std), and select features (L1, SBS, RF). Experiments showed preprocessing improves model performance

Experiment with Iris Dataset:
-Load via from sklearn.datasets import load_iris.
-Apply similar steps: Impute (if add missing), encode (no categoricals), split, scale, select.
-Effect: Scaling boosts KNN/SVM accuracy; selection reduces dims from 4 to 2-3 without loss.


Questions:

1. Why is handling missing data important?

Missing values cause errors in algorithms or biased models. Handling ensures complete, unbiased data.

2.When should you use one-hot encoding vs. label encoding? 

One-hot for nominal (unordered, e.g., colors) to avoid implied order. Label for ordinal (ordered, e.g., sizes) or targets.

3.How does feature scaling impact algorithms like KNN or SVM? 

They are distance-based; unscaled features dominate (e.g., large-range feature overshadows others). Scaling equalizes influence, improving accuracy.

4.Compare L1 regularization and SBS for feature selection. 

L1 (lasso) shrinks coeffs to zero implicitly (sparsity via penalty, fast for high-dims). SBS explicitly removes features stepwise (greedy, evaluates subsets, better for small datasets but computationally expensive).
