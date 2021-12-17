# Customer Churn Prediction Modelling and the Impact of Adversarial Machine Learning Attacks on the Performance of the Models
![Churn image](https://res.cloudinary.com/dn1j6dpd7/image/fetch/f_auto,q_auto,w_736/https://www.livechat.com/wp-content/uploads/2016/04/customer-churn@2x.jpg)

In an era when markets are becoming increasingly saturated and the competition between businesses continue to intensify, customer churn presents a real problem. It has become apparent to business owners that for their companies to compete favourably, there is a need to implement carefully thought-out customer retention strategies that seek to initiate, maintain, and strengthen long-lasting relationships with customers (Torkzadeh, Chang, & Hansen, 2006).This is especially applicable in highly competitive, subscription-based service industries such as the telecommunication industry.
Customer retention is very important and remains the topmost priority of companies and while there are indeed many reasons for this, the following
reasons are worth noting:
1. Cost of getting new customers
2. Social network influence
3. Long term customers are more beneficial
4. Competition has less effect on loyal customers

As businesses continue to rely on machine learning models for automated churn prediction, it should be taken into account that there have been emerging
concerns about the vulnerability and robustness of machine learning systems. Incentivised attackers may seek to manipulate the performance of a model, causing it to malfunction by providing deceptive input and this is known as an adversarial attack.

# Objectives
The objective of this project is to:

• Use data analytic insights to Understand drivers of churn

• Design and implement ML models and adversarial machine learning experiments to understand model robustness.

• Critically analyse and discuss results obtained from implemented adversarial experiments.

• Draw conclusions from analysis made and recommend future research based on limitations.

# Modelling

Modelling was carried out using:

• Logistic regression (Conditional probability = 0.5)

<img src="https://miro.medium.com/max/720/1*CYAn9ACXrWX3IneHSoMVOQ.gif" width="400">

• Support Vector Classifier (Kernel=RBF, C=40, gamma=0.01)

<img src="https://c.mql5.com/2/5/svmregression.gif" width="300">

• Artificial neural network (Layer 1 = 100 neurons, Layer 2= 100 neurons, Layer 3= 100 neurons, Activation = Relu, Loss = Categorical crossentropy, Optimizer = Adam)

<img src="https://miro.medium.com/max/788/1*F5IKudcD4acJb0hcfoIVdA.gif" width="400">

# Attacks

• Fast Gradient Sign Method(epsilon=0 to 1)

• Deep Fool Attack (epsilon=0 to  0.00001)

• Jacobian Saliency Map Attack (gamma=1%, theta=0 to 1)

# Results and conclusions
<img src="https://github.com/ezraabah/Customer-churn-prediction-modelling-and-impact-of-Adversarial-ML-Attacks-on-model-performance/blob/main/image30.png" width="600">
An analysis of results obtained by evaluating the performance of the models showed that in the absence of adversaries, logistic regression outperforms other models followed by artificial neural network and finally support vector classifier. However, in the presence of adversarial attacks, support vector classifier performed the best thus proving its robustness to adversaries. This was followed by artificial neural network and logistic regression models consecutively, both of which performed poorly and showed vulnerability to adversarial attacks. On that basis, it is recommended that support vector machine algorithm is used when deploying customer churn prediction classifiers in potentially adversarial environments.
