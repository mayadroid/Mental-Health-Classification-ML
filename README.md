# Mental-Health-Classification-ML
Mental Health Classification using Machine Learning

In this study, we aim to develop data mining models for the classification of the risk for poor mental health. We will be
focussing on people working in tech roles/industry. The models will be developed with datasets obtained from
OSMH/OSMI Mental Health in Tech Survey. This raw dataset spans 5 years from 2017 to 2021 and has 124 variables
including demographics (age and gender), geography (country and state of residence), working in a tech company, seeking
help in the workplace, and presence of any treatment. Out of 124 variables, we will be using 21 variables, which we
found worth including in our study, as mentioned below:
Dependent variable:
MH_disorder  (whether this person currently has mental health disorder)
Independent variables:
Personal Information (7):
age, gender, country, past_disorder, family_history, treatment, IT_related. (currently doing IT related positions)
Working Company Information & Provided Healthcare Resources (13):
company_size, HC_coverage (HealthCare coverage), medical_leave (for mental health issue), PH_importance (physical
health), MH_importance (mental health), observation, unsupported_space, supported_space, tech_support (how well the
tech companies support MH issues), coverage_option, formal_discussion, resources, employer_discussion.

The models we used for mental health classification are:
1. Logistic Regression
2. Random Forest
3. Boosting
4. KNN
5. Naive Bayes
6. Classification Tree
7. Clustering
8. Association Rule

After experimenting with different models and variables, we decided to build our models without the “country” variable.
The main reason is that most of our models cannot handle text features, and we cannot treat it as a categorical feature
since there are too many countries. Also, after sampling, the test data might have some countries that the train data does
not have which leads to mismatch of levels. We have used 70/30 partitioning while splitting the train and test data from
the dataset.
