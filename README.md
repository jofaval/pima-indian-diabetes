# Pima Indian Diabetes - Data Analysis #

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jofaval/pima-indian-diabetes/blob/master/notebook.ipynb)&nbsp;[![Open in Kaggle](https://www.kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/jofaval/distributed-approach-diabetes-detection-0-96-auc)

## Table of contents

1. [📁 Data](#-data)
1. [📓 Description](#-description)
1. [✔️ Objective](#-objective)
1. [🧱 Tech stack](#-tech-stack)
1. [💹 Algorithms](#-algorithms)
1. [📊 Visualization](#-visualization)
1. [🤓 Conclusions](#-conclusions)
1. [©️ Credits](#-credits)

## 📁 Data
[↑ Back to the table](#table-of-contents)

The data is available at the official archive link:\
[https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

## 📓 Description
[↑ Back to the table](#table-of-contents)

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.

## ✔️ Objective
[↑ Back to the table](#table-of-contents)

To predict as closely as possible wether a woman above 21 years of age has or will have diabetes.

Understanding what contributes to it is also a plus, but there's two factors that don't allow it:

- My lack of knowledge and expertise in the health field
- The lack of information and more samples for this dataset and particular case. Such as: nutrition, genetic heritage, work status, stress, mental health, physical activity, to name a few.

## 🧱 Tech stack
[↑ Back to the table](#table-of-contents)

Python, that's it! R is a programming language that, as for the moment being, I have no experience with, even though it's powerful and broadly used, but I'd dare to say that no more than Python.

And one of the strongest points, if not the most, about Python, are it's libraries, so... the libraries I've used are:

- Pandas, data manipulation with an ease of use and exploration data analysis.
- Numpy, a really strong linear algebra library, used in the project for it's statistics utilities, SciPy may be an alternative, but I have no experience at all with it.
- Matplotlib and Seaborn, both fantastic libraries for data visualization, and they complement each other.
- Scikit-Learn, the library used for Machine Learning and statistics models: Linear Regression, SVR, Lasso, Ridge, etc.

## 💹 Algorithms
[↑ Back to the table](#table-of-contents)

- **Polynomial Logistic Regression**, always start with the basics, it's surprising how effective the simplest of the solutions usually are, Logistic Regression is Linear Regression with a logarithmic function applied to it's outcome to ensure a binary response, which means that we can add polynomial degrees to it's linear resolution as to improve it's understanding of the problem. Which turned out great
- **KNearest-Neighbour**, imitating real life, near data tend to be similar, in other words, if a row is close (statistically speaking) to another row, there's a chance it will also be of the same label.
- **Naive Bayes**, a probabilistic approach based on the Bayes' Theorem that the probability of an occurence may contribute to the probability of another event, it performed really great on unbalanced sets, but it was not the best fit for this project when the data was balanced
- **Random Forest Classifier**, at times one of the best, but was outperformed but other algorithms, still, a top five for this project and a powerful technique
- **Deep Learning Neural Networks**, Deep Learning here did not perform great, most likely because it required of more data to actually learn the patterns
- **XGBoost Classifier**, a surprisingly efficient solution that, no matter if balanced or unbalanced, actually remained sort of unbiased and, while not having the highest score, performed greatly and consistently at the confusion matrix

F1 score wasn't really great for our metrics here, what did gave an insight was the confusion matrix, since many models actually just return either all ones or all zeros. But balancing the data helped a lot fixing that.

## 📊 Visualization
[↑ Back to the table](#table-of-contents)

Normalized confusion matrices, lineplots, correlation (heatmap) plot with an identity matrix applied, pie charts and boxplots to better analyze the data distribution.

But there were no crazy visualizations for this project, if something, the age and pregnancies hypothesis evaluation one, where age and pregnancies where plotted together to see there correlation between diabetes. But it did shocked me the amount of pregnancies.

## 🤓 Conclusions
[↑ Back to the table](#table-of-contents)

Whenever possible, even on a perfect, ready-to-work dataset, read the abstract, the paper, whatever information it is that you may have at hand, it truly helps understand the evaluation of the results and it's tuning.

Distribution, once again, helps a lot, but understanding the problem you're tackling helps even more, my work wasn't the best, but I do believe it's quite good as a data science approach, but the data analysis part has a lot of room for improvement. But, my lack of knowledge and understanding of the field really did take a hit on this project, that's for sure.

And the best notebook I saw, a notebook by [vincentlugat](https://www.kaggle.com/code/vincentlugat), [Pima Indians Diabetes - EDA & Prediction (0.906)](https://www.kaggle.com/code/vincentlugat/pima-indians-diabetes-eda-prediction-0-906) was an incredibly and extensive analysis. It proved how understanding the problem you're tackling while doing a data analysis can actually get the best result. And, if something, it's worth a read, no matter if you're intrested in the dataset, or data science in general.

## ©️ Credits
[↑ Back to the table](#table-of-contents)

National Institute of Diabetes and Digestive and Kidney Diseases.

Smith, J.W., Everhart, J.E., Dickson, W.C., Knowler, W.C., & Johannes, R.S. (1988). Using the ADAP learning algorithm to forecast the onset of diabetes mellitus. In Proceedings of the Symposium on Computer Applications and Medical Care (pp. 261--265). IEEE Computer Society Press.

Uploaded at Kaggle, a company owned by Google by [https://www.kaggle.com/uciml](https://www.kaggle.com/uciml).

I'd also like to credit [vincentlugat](https://www.kaggle.com/code/vincentlugat), not because I took inspiration or something, but it was a nice experience overall to see such as detailed notebook and hardworked approach.