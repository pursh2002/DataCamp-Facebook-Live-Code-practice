My machine learning/data science workflow that I've been practicing for years (Part 1):

1. Scoping:

First you scope the problem that you want to solve. Is that a classification or clustering problem? Do you have enough data? If not can we collect it. API First - where will our machine model be used? What is the latency requirement? How can we re-train our model? What is a good model evaluation?

2. Data Review:

Jupyter Notebook and "import pandas as pd" are my best friends. Do a lot of summaries (min, max, mean, median etc.). Check for outliers. Understand the definition of each column. For classification, check target variables. A lot of plots... matplotlib and seaborn FTW

3. Feature Engineering:

Normalize data, convert data so that it can be used by scikit-learn e.g. one-hot encoding for categorical variables or text data into vectors (bag of words, tf-idf), clean data etc...

4. Feature Review:

Review transformed input data before the modelling. A lot of errors can happen during a transformations e.g. in one hot encoding we forgot one column...

Please kindly share it if you find this workflow useful! Tarry Singh, Han Xiao, Eric Weber, Kyle McKiou, Mike Richardson (迈克尔), Andriy Burkov

P.S. LinkedIn has a limit on characters. 
Here's Part 2: https://lnkd.in/gFcGViR