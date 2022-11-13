# Churn-Prediction

Date: 30.09.2021

Problem statement: You are given data of 1.000 users for period of 3 years. The data includes information about the phone calls, SMSes and data usage for each user during their subscription period. Your task is to make a model that based on the history of the user, predicts whether the user will terminate the subscription or not.

You are given the following 6 files:
1.	personal_info.tsv. The format of this file is (id, birth date, gender, subscription_start_date, subscription_end_date). Every row represents a user and their subscription period.
2.	contract_info.tsv. The format of this file is (id, contract_start_date, contract_end_date). A customer may have multiple or may not have multiple contracts during their subscription period.
3.	phone_calls.tsv. The format of this file is (id, date, duration, operator, roaming). A single entry in the file represents total duration duration (in seconds) of all calls the customer with ID id made towards customers of operator operator on date date. The flag roaming indicates whether the call was in roaming mode.
4.	sms.tsv. The format of this file is (id, date, num, operator, roaming). A single entry in the file represents total number of SMSes sms the customer with ID id made towards customers of operator operator on date date. The flag roaming indicates whether the SMSes were sent in roaming mode.
5.	data.tsv. The format of this file is (id, date, size, operator, roaming). A single entry in the file represents total amount of data data (in MB) the customer with ID id made on date date. The flag roaming indicates whether the data was used in roaming mode. When it is 0, the operator is also 0 representing our operator.
6.	invoice.tsv. The format of this file is (id, month, amount). A single entry describes that the customer with ID id had an invoice of amount EUR for month month.
