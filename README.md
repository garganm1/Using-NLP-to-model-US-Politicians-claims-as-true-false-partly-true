# Using-NLP-to-model-claims-as-true-false-partly-true

The project focuses on implementing Natural Language Processing on a dataset consisting of claims and a list of articles supporting those claims, thereby developing a supervised machine learning model that will be able to predict the measure of truthness of each claim from one of the three categories namely "True", "Partly True" and "False".

Extending further, considering the claim labels in the dataset as "ground truth", we analyse the predictions of claims made by prominent US politicians to deduce the degree of fake news being spread.

Explaining Dataset: The dataset contains datapoints that contains a claim in text form taken from a set of "ground truth" articles. The claim could have been manipulated to denote as a fake claim or it could be a true claim or partly true claim. There is a date of claim, name of the claimant who made the claim and the label of the claim i.e. false, true or partly true.

We bifurcate the project into following sections:
1. Data Exploration
2. Data Cleaning
3. Model Preparation
4. Model Implementation
5. Discussions & Results

Upon Data Exploration, we find that US politicians such as Donald Trump, Hillary Clinton and Barack Obama are some of the claimants who have a huge count of claims. So, it was decided to extract their claims from the dataset such that their claims act as testing set and the remaining claims act as training set for the model to generalize upon.

Both the claims and articles (in text format) were cleaned through NLP techniques and both are combined to vectorize using TF-IDF. We implement four models (Random Forest, XGBoost, SVM & Logistic Regression) to check which ML algorithm works best for our dataset.

The results showed some concerning inferences. It showed that the count of false claims made by the US politicians have been ever-increasing over the years since 2015 and the lion's share of these false claims were made by Donald Trump (current US sitting president). The proliferation of these false claims have not stopped even after the 2016 US elections suggesting a lack of awareness and/or technology debunking these claims in real-time.

If you find this interesting, do have a look at the notebook!
