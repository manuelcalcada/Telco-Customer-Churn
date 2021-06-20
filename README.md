# Telco Customer Churn

![image](https://user-images.githubusercontent.com/42875146/122658938-f1d43980-d148-11eb-857a-25ae5b448e3c.png)

## Objective
To predict the behavior of customers who will be churn in the next month in order to retain those customers by analyze all relevant customer data and develop focused customer retention programs.

## Used data
- Each row represents a customer.
- Each column contains customer’s attributes.
- The data set includes information about:
    - Customers who left within the last month – the column is called Churn
    - Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies
    - Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges
    - Demographic info about customers – gender, age range, and if they have partners and dependents
- The used dataset was obtained in https://www.kaggle.com/blastchar/telco-customer-churn

## Hypothesis
Some hypotheses were formulated to predict the behavior of customers who are likely to churn or not in the next month.
These hypotheses were divided into three groups:
 1. Services information hypotheses
     - These hypotheses are related to the customer contacted products and services
 1. Customer information hypotheses
     - These hypotheses are related to the customer account information, like contract, payment method and charges
 1. Sociodemographic information hypotheses
     - These hypotheses are related to the customer sociodemographic information, like gender, age and so on

<br>
<table>
	<thead>
        <tr>
			<th colspan = "3" style="text-align:center;">Hypotheses summary</th>
		</tr>
		<tr>
			<th>Group</th>
			<th>#</th>
			<th>Hypothesis</th>
		</tr>
	</thead>
	<tbody>
		<tr style="background-color:#99a9cc;">
            <td rowspan="9" style="background-color:#99a9cc;"><strong>Services <br> informations</strong></td>
			<td><strong>H1</strong></td>
			<td style="background-color:#99a9cc;">Customers with phone services are less likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H2</strong></td>
			<td>Customers with fewer phone lines are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H3</strong></td>
			<td>Customers with internet services are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H4</strong></td>
			<td>Customers with online security service are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H5</strong></td>
			<td>Customers with online backup service are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H6</strong></td>
			<td>Customers with device protection service are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H7</strong></td>
			<td>Customers with tech support service are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H8</strong></td>
			<td>Customers with TV streaming service are more likely to churn</td>
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H9</strong></td>
			<td>Customers with movie streaming service are more likely to churn</td>
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td rowspan="6"><strong>Customer <br> informations</strong></td>
            <td><strong>H10</strong></td>
			<td>Customers with a longer relationship with the company are less likely to churn</td>
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H11</strong></td>
			<td>Customers monthly contract are more likely to churn</td>
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H12</strong></td>
			<td>Customers with paperless billing are more likely to churn</td>
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H13</strong></td>
			<td>Customers with automatic payment methods are less likely to churn</td>
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H14</strong></td>
			<td>Customers with less monthly expenses are less likely to churn</td>
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H15</strong></td>
			<td>Customers with less total expenses are less likely to churn</td>
		</tr>
		<tr style="background-color:#aeb9d1;">
			<td rowspan="4"><strong>Sociodemographic <br> informations</strong></td>
            <td><strong>H16</strong></td>
			<td>Female customers are less likely to churn</td>
		</tr>
		<tr style="background-color:#aeb9d1;">
            <td><strong>H17</strong></td>
			<td>Senior citizen customers are less likely to churn</td>
		</tr>
		<tr style="background-color:#aeb9d1;">
            <td><strong>H18</strong></td>
			<td>Customers with partners are more likely to churn</td>
		</tr>
		<tr style="background-color:#aeb9d1;">
            <td><strong>H19</strong></td>
			<td>Customers with dependents are more likely to churn</td>
		</tr>
	</tbody>
</table>

## Methodology

The methodology used in the analysis of this case will be the CRISP-DM, through the following division of scripts (click to go to the notebook):
1. [Exploratory Data Analysis - Business and Data understanding](https://github.com/manuelcalcada/Telco-Customer-Churn/blob/main/1.%20EDA/Telco_churn%20-%20EDA.ipynb "EDA notebook") 
2. [Data pre-processing - Data preparation](https://github.com/manuelcalcada/Telco-Customer-Churn/blob/main/2.%20Pre-processing/Telco_churn%20-%20Data%20pre-processing.ipynb "Data pre-processing notebook")
3. [Statistical modeling of a churn propensity model - Modeling and Evaluation](https://github.com/manuelcalcada/Telco-Customer-Churn/blob/main/3.%20Churn%20propensity%20model/Telco_churn%20-%20Churn%20propensity%20model.ipynb "Classification notebook")
4. [Statistical modeling of a regression model of the customer charge - Modeling and Evaluation](https://github.com/manuelcalcada/Telco-Customer-Churn/blob/main/4.%20Customer%20charge%20model/Regression%20model%20of%20the%20customer%20charge.ipynb "Regression notebook")
5. [Statistical modeling of a customer clustering model - Modeling and Evaluation](https://github.com/manuelcalcada/Telco-Customer-Churn/blob/main/5.%20Customer%20clustering%20model/Customer_clustering_model.ipynb "Clustering notebook")

## Exploratory Data Analysis main results

![image](https://user-images.githubusercontent.com/42875146/122677343-59759d80-d1b8-11eb-99af-a40f2dc16385.png)

![image](https://user-images.githubusercontent.com/42875146/122677347-5d092480-d1b8-11eb-8495-cdda778690ca.png)

![image](https://user-images.githubusercontent.com/42875146/122677349-60041500-d1b8-11eb-849f-79a314c7427f.png)

### Insights from bivariate analysis

- Customers with phone service seem to have a slightly greater propensity to churn than others
- Customers with multiple phone lines seem to have a slightly greater propensity to churn than others
- Customers with fiber optic internet service seem to have a greater propensity to churn than DSL customers. Also, customers with internet services seem to have a greater propensity to churn than others
- Customers without online security, online backup, device protection, and tech support services seem to have a slightly greater propensity to churn than others
- Customers without TV streaming and movies streaming seem to have a greater propensity to churn than other customers
- Customers with less tenure seem to have a greater propensity to churn than others
- Customers with lower monthly charges seem to have a lower propensity to churn than others
- Month-to-month customers seem to have a greater propensity to churn than others
- Paperless billing customers seem to have a greater propensity to churn than others
- Customers with eletronic check payment method seem to have a greater propensity to churn than others
- Customers with automatic payment method seem to have less propensity to churn than others
- There are no significant differences between the two groups in the gender variable
- Senior citizens seem to have a greater propensity to churn than others
- Customers without partner seem to have a greater propensity to churn than others
- Customers without dependents seem to have a greater propensity to churn than others

## Churn propensity model

The following models was used:

1. Logistic Regression
1. K-Nearest Neighbors
1. Decision Tree
1. Gaussian Naive-Bayes
1. Suport Vector Machine
1. Gradient Boosting
1. Extra Trees
1. Ada Boost
1. Stochastic gradient descent
1. Random Forest
1. XGBoost
1. Multi Layer Perceptron Neural Network

The model training and evaluate followed the steps below:

1. **Scenery 1.1**: Training all the models with the default hyperparameters in the original dataset
1. **Scenery 1.2**: Training all the models with the default hyperparameters in the dataset with tenure as categorical
1. **Scenery 1.3**: Training all the models with the default hyperparameters in the original dataset after PCA transformation
1. **Scenery 1.4**: Training all the models with the default hyperparameters in the original dataset after SMOTE balancing
1. **Scenery 1.5**: Training all the models with the default hyperparameters in the original dataset after undersampling balancing
1. **Scenery 1.6**: Training all the models with the default hyperparameters in the original dataset after feature selection
1. **Scenery 2.1**: Training all the models with the default hyperparameters using the best three founded scenarios
1. Hyperparameter optimization of the best models found in the best scenario
1. Creation of voting classifiers with these best models
1. Definition of the chosen model

The models evaluation focus mainly in:
1. F1-Score (test partition)
1. Precision (test partition)
1. Cross validation accuracy (in train partition)
1. Stability (in cross validation train and the whole sample train)
1. Accuracy (test partition)

### Best model and scenario results

#### Confusion matrix

![image](https://user-images.githubusercontent.com/42875146/122677686-bcb3ff80-d1b9-11eb-9863-6bbdf41d34c0.png)

#### Feature importance

![image](https://user-images.githubusercontent.com/42875146/122677712-dfdeaf00-d1b9-11eb-927a-0e46ccf4a03f.png)

So, for this model, the most important feature was the tenure. The higher the tenure, the lower the churn propensity. This is inline with the EDA insights and the hypothesis.

#### Decile analysis

![image](https://user-images.githubusercontent.com/42875146/122659082-36aca000-d14a-11eb-8f77-f1959c3122a1.png)

According to the lift, the first two deciles are highly important to be encouraged by a marketing campaign in order to stay in the company and not go into churn. The third and fourth deciles also have a higher churn average than the total base average, so they should also be reached by a marketing campaign.

## Charge regression model

The following models was used:

1. Linear regression (OLS)
1. Logistic Regression
1. K-Nearest Neighbors
1. Decision Tree
1. Gaussian Naive-Bayes
1. Suport Vector Machine
1. Gradient Boosting
1. Extra Trees
1. Ada Boost
1. Stochastic gradient descent
1. Random Forest
1. XGBoost
1. Multi Layer Perceptron Neural Network

The model training and evaluate followed the steps below:

1. Training all the models with the default hyperparameters in the original dataset
1. Hyperparameter optimization of the best models found (if needed)
1. Creation of voting regressors with these best models (if needed)
1. Definition of the chosen model

The models evaluation focus mainly in:
1. R2-score (test partition)
1. MAE (test partition)
1. MSE (test partition)

### Best model and scenario results

The best model was a linear regression.

In this experiment, a regression model was created to predict the monthly charge paid by the customer. This model is useful to be used with the churn propensity model, in the final table of propensity, where it can be compared if the value of the customer prone to churn is outdated (greater) than that of customers who are not prone.

In this way, we were also able to understand the impact on cost that each service purchased has, as well as their combination in bundle.

## Customer clustering model

Using an elbow method, the KN clustering founds 4 clusters to the customers.

![image](https://user-images.githubusercontent.com/42875146/122659571-d15bad80-d14f-11eb-9cea-49aeca7e8bee.png)

**From these analysis**:

 Cluster 0:
  - The customers are younger than clusters 1 and 3
  - Has more phone services than internet services
  - Has usually one phone line
  - Customers with approximately 3 years of tenure
  - Has a low term contract (monthly)
  - Uses an electronic check payment method
  - Uses as much fiber optic internet as DSL internet
  - Spends an average of 62 dollars per month

 Cluster 1:
  - Higher percentage of senior citizens than other clusters
  - Higher percentage of married people with dependents
  - Higher tenure (more than 5 years)
  - Has all the internet and phone services
  - Has multiple phone lines 
  - Uses a fiber optic internet
  - Higher monthly charges than others clusters
  - Spends an average of 100 dollars per month
  - Has paperless billing
  - High use of TV and movie streaming
  - Has a long term contract (2 years)
  - Uses an automatic payment method
  - Less propensity to churn

 Cluster 2:
  - Younger customers
  - Has more phone services than internet services
  - Has one phone line
  - Customers with less than 1 year of tenure
  - Has a low term contract (monthly)
  - Uses an electronic check and mailed check payment method
  - Uses as much fiber optic internet as DSL internet
  - Spends an average of 48 dollars per month
  - High propensity to churn

 Cluster 3:
  - Has more internet services than phone services
  - Has more than one phone line
  - Customers with 4 years of tenure
  - Has a mid term contract (1 year)
  - Uses an electronic check payment method
  - Uses a fiber optic internet
  - Spends an average of 82 dollars per month
  
  
  --- 
  Visit my [LinkedIn](https://www.linkedin.com/in/manuelcalcada/ "Stay in touch!")!
