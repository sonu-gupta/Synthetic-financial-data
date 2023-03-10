# Synthetic Financial Data Generation for Fraud Detection

I used the credit card fraud dataset from <a href="https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud" target="_blank">Kaggle</a> (published by ULB).

About Dataset: It includes information on credit card transactions carried out by cardholders in Europe during September 2013. The data pertains to a two-day period and shows that out of 284,807 transactions, 492 were fraudulent. The dataset is imbalanced as the fraud cases represent only 0.172% of all transactions.

One way to handle this data imbalance is to synthesize the data for minority class. Synthetic data generators utilize actual data to identify pertinent characteristics, relationships, and trends so as to produce sufficient amounts of synthetic data that matches the statistical characteristics of the initially collected dataset. Here, I've used Wasserstein GAN - Gradient Penalty (WGAN-GP). It is a type of generative adversarial network (GAN) that leverages the Wasserstein loss formulation in combination with a penalty on gradient norm to attain Lipschitz continuity.

The code is adapted from: 
<a href="https://aws.amazon.com/blogs/machine-learning/augment-fraud-transactions-using-synthetic-data-in-amazon-sagemaker/" target="_blank">AWS Machine Learning</a>

In progress: Evaluation of the quality of synthetic dataset.
