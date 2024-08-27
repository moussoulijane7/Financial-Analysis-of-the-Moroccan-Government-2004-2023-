# Financial-Analysis-of-the-Moroccan-Government-2004-2023-
Introduction
The objective of this project is to analyze and forecast the financial data of the Moroccan government from 2004 to 2023. This analysis involves examining key financial indicators, detecting anomalies, and predicting future trends using various time series models. The dataset includes the following key financial variables:

Variables
Date:
The date on which the financial data was recorded. This serves as the time index for the dataset.

IS (Impôt sur les Sociétés - Corporate Tax):
This variable represents the taxes levied on corporate profits. It is a major source of government revenue.

IR (Impôt sur le Revenu - Income Tax):
The tax collected on individual income, which includes salaries, wages, and other earnings. It is another crucial source of state revenue.

TVA (Taxe sur la Valeur Ajoutée - Value-Added Tax):
A consumption tax placed on a product whenever value is added at each stage of the supply chain, from production to the point of sale.

TIC (Taxe Intérieure de Consommation - Domestic Consumption Tax):
This tax is imposed on specific goods, often including fuel, alcohol, and tobacco, and is a significant component of indirect taxation.

BetS (Dépenses en Biens et Services - Expenditure on Goods and Services):
Government spending on goods and services necessary for public service delivery, including healthcare, education, and infrastructure.

intD (Intérêt de la Dette - Debt Interest):
The interest payments made by the government on its outstanding debt. This variable reflects the cost of borrowing and managing national debt.

COMP (Compensation):
This represents the total compensation, including salaries and wages, paid to government employees. It is a significant component of public expenditure.

Methodology
In this project, we used the following methodologies:

Descriptive Analysis:
To identify general trends and correlations in the historical financial data.

Anomaly Detection:
The Isolation Forest algorithm was applied to automatically detect anomalies in the data, which could indicate irregularities or significant events.

Predictive Modeling:
Time series forecasting models such as ARIMA, VAR, and LSTM were used to predict future financial trends based on the historical data.

Evaluation Metrics
Each model was evaluated using the following performance metrics:

RMSE (Root Mean Squared Error):
A measure of the differences between predicted and observed values, indicating the model's accuracy.

MAPE (Mean Absolute Percentage Error):
A measure of prediction accuracy in forecasting models, showing the average absolute percentage difference between predicted and actual values.
