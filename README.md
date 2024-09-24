# Bank-customers-EDA-analysis-and-segmentation
The purpose of my project is to master EDA using banking dataset.
The goals of the project:
1) to clean and to explore the dataset with pandas
2) to visualize the data with the various plot types
3) to provide RFM analysis of bank's customer base 
4) to explore customers' loyalty to bank's products.

In the project I gave answers to a set of questions that relevant to banking and marketing topics:
1) What is a geographical distribution of customers as well as their age and gender distribution?
2) What is the average value for balance-to-transaction ratio for different age groups?
3) What is a correlation between numerical data?
4) What tendencies can be observed? I visualized tendencies and this can help to plan marketing campaigns more effectively.

The dataset includes more than 1 M rows so python is the preferable tool to be used for data manipulation.
The dataset contains the following information about bank's transactions: customerID, customer gender, customer location, date of birth, account balance, transaction ID, transaction amount, transaction date, transaction time.

First of all the main statistic parameters were calculated for numerical and non-numerical columns. This revealed some illogic in data: transaction amount can't be equal 0, transaction time can't be equal 0. As well as the age can't be a negative number. These illogic patterns were deleted from the dataset.
Then the distribution of different variables was checked: distribution of customers' location, age, gender, distribution of customers' account balances and transaction amounts, number of transactions by months and daytime.

The conclusions of the EDA analysis:
1) The average balance-to-transaction ratio is greater for young customers (under 35) and it decreases for older persons. This proves that young people make transactions more frequently. This group might benefit from such services as digital banking and mobile transactions.
2) The greatest number of transactions appeared in August but the average transaction amount was almost equal every months.
3) The greatest number of transactions was held at night, the second greatest - in the morning. This info is helpful for marketing campaigns' planning.

For conducting RFM analysis all clients were divided according to the recency of their transactions (R1 - earlier than 1 month), frequency (F1 - 5 or more transacions), monetary input (M1 - transaction amount greater than 400 INR).
The conclusions of the RFM analysis:
1) Clients are not very loyal (because there are not many clients in group R1).
2) The RFM analysis of transactions shows that customers who performed the largest transactions carried out them long ago (more than 6 months) - R3F3M1. It's doubtful if it's worth spending marketing budget on such customers.
3) Good customers are R1F2M1 and R1F2M2 but there are not many of them (1% of total customers).
4) The second largest group R3F3M3 consists of the worst customers and accounts for 172.8 thousand clients. It's useless spending money on attracting them.
5) The advice is to stimulate groups R1F3M1 and R1F3M2 (884 thousand clients, 15% of total) through marketing campaigns.
