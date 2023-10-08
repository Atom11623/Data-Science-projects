### Churn Analysis: Exploratory Data Analysis
## Introduction
This exploratory data analysis aims to uncover insights into customer churn for a utility company. The analysis encompasses historical customer data, pricing information, and a churn indicator. Understanding the underlying factors influencing churn is crucial for devising effective customer retention strategies.

## Dataset Description
client_data.csv
id: Client company identifier
activity_new: Category of the company’s activity
channel_sales: Code of the sales channel
cons_12m: Electricity consumption of the past 12 months
cons_gas_12m: Gas consumption of the past 12 months
cons_last_month: Electricity consumption of the last month
date_activ: Date of activation of the contract
date_end: Registered date of the end of the contract
date_modif_prod: Date of the last modification of the product
date_renewal: Date of the next contract renewal
forecast_cons_12m: Forecasted electricity consumption for next 12 months
forecast_cons_year: Forecasted electricity consumption for the next calendar year
forecast_discount_energy: Forecasted value of current discount
forecast_meter_rent_12m: Forecasted bill of meter rental for the next 2 months
forecast_price_energy_off_peak: Forecasted energy price for 1st period (off peak)
forecast_price_energy_peak: Forecasted energy price for 2nd period (peak)
forecast_price_pow_off_peak: Forecasted power price for 1st period (off peak)
has_gas: Indicated if client is also a gas client
imp_cons: Current paid consumption
margin_gross_pow_ele: Gross margin on power subscription
margin_net_pow_ele: Net margin on power subscription
nb_prod_act: Number of active products and services
net_margin: Total net margin
num_years_antig: Antiquity of the client (in number of years)
origin_up: Code of the electricity campaign the customer first subscribed to
pow_max: Subscribed power
churn: Has the client churned over the next 3 months

## price_data.csv

id: Client company identifier
price_date: Reference date
price_off_peak_var: Price of energy for the 1st period (off peak)
price_peak_var: Price of energy for the 2nd period (peak)
price_mid_peak_var: Price of energy for the 3rd period (mid peak)
price_off_peak_fix: Price of power for the 1st period (off peak)
price_peak_fix: Price of power for the 2nd period (peak)
price_mid_peak_fix: Price of power for the 3rd period (mid peak)

## EDA Summary
Findings
Approximately 10% of customers have churned.
Consumption data is highly skewed and must be treated before modeling.
Outliers are present in the data and should be addressed before modeling.
Price sensitivity exhibits a low correlation with churn.
Feature engineering will be vital, especially for enhancing the predictive power of price sensitivity.

## Suggestions
Competitor Price Data:

Consider incorporating competitor price data. Clients may be more inclined to churn if a competitor offers a compelling deal.
Average Utilities Prices Across the Country:

Analyze average utility prices across the country. Significant deviations from the country average might influence a client's likelihood to churn.
Client Feedback:

Explore client feedback, including complaints, calls, or other interactions with PowerCo. This information may provide valuable insights into a client's propensity to churn.
Conclusion
This exploratory data analysis lays the foundation for further in-depth analysis and modeling efforts to understand and mitigate customer churn. It is recommended to explore additional data sources and perform advanced feature engineering to improve the predictive accuracy of churn models. By implementing the suggested enhancements and strategies, PowerCo can effectively enhance customer retention efforts and sustain business growth.
