# Telco Customer Churn

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

<table>
	<thead>
        <tr>
			<th colspan = "4" style="text-align:center;">Hypotheses summary</th>
		</tr>
		<tr>
			<th>Group</th>
			<th>#</th>
			<th>Hypothesis</th>
            <th>Result</th>
		</tr>
	</thead>
	<tbody>
		<tr style="background-color:#99a9cc;">
            <td rowspan="9" style="background-color:#99a9cc;"><strong>Services <br> informations</strong></td>
			<td><strong>H1</strong></td>
			<td style="background-color:#99a9cc;">Customers with phone services are less likely to churn</td>
            <td style="background-color:#32a852;">Accepted</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H2</strong></td>
			<td>Customers with fewer phone lines are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H3</strong></td>
			<td>Customers with internet services are more likely to churn</td>
            <td style="background-color:#32a852;">Accepted</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H4</strong></td>
			<td>Customers with online security service are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H5</strong></td>
			<td>Customers with online backup service are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H6</strong></td>
			<td>Customers with device protection service are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H7</strong></td>
			<td>Customers with tech support service are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H8</strong></td>
			<td>Customers with TV streaming service are more likely to churn</td>
            <td style="background-color:#a8a7a7;">-</td> 
		</tr>
		<tr style="background-color:#99a9cc;">
            <td><strong>H9</strong></td>
			<td>Customers with movie streaming service are more likely to churn</td>
            <td style="background-color:#a8a7a7;">-</td> 
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td rowspan="6"><strong>Customer <br> informations</strong></td>
            <td><strong>H10</strong></td>
			<td>Customers with a longer relationship with the company are less likely to churn</td>
            <td style="background-color:#32a852;">Accepted</td> 
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H11</strong></td>
			<td>Customers monthly contract are more likely to churn</td>
            <td style="background-color:#32a852;">Accepted</td> 
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H12</strong></td>
			<td>Customers with paperless billing are more likely to churn</td>
            <td style="background-color:#32a852;">Accepted</td> 
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H13</strong></td>
			<td>Customers with automatic payment methods are less likely to churn</td>
            <td style="background-color:#32a852;">Accepted</td> 
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H14</strong></td>
			<td>Customers with less monthly expenses are less likely to churn</td>
            <td style="background-color:#a8a7a7;">-</td> 
		</tr>
		<tr style="background-color:#a3b1cf;">
            <td><strong>H15</strong></td>
			<td>Customers with less total expenses are less likely to churn</td>
            <td style="background-color:#a8a7a7;">-</td> 
		</tr>
		<tr style="background-color:#aeb9d1;">
			<td rowspan="4"><strong>Sociodemographic <br> informations</strong></td>
            <td><strong>H16</strong></td>
			<td>Female customers are less likely to churn</td>
            <td style="background-color:#a8a7a7;">-</td> 
		</tr>
		<tr style="background-color:#aeb9d1;">
            <td><strong>H17</strong></td>
			<td>Senior citizen customers are less likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td>
		</tr>
		<tr style="background-color:#aeb9d1;">
            <td><strong>H18</strong></td>
			<td>Customers with partners are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td>
		</tr>
		<tr style="background-color:#aeb9d1;">
            <td><strong>H19</strong></td>
			<td>Customers with dependents are more likely to churn</td>
            <td style="background-color:#eb4034;">Rejected</td>
		</tr>
	</tbody>
</table>
