# Project Capstone: Market Segmentation 

## Executive Summary
This study seeks to develop a model capable of segregating customers so as to help insurance companies creating relevant offers that provide high-value experiences to customers that translates to increase in customer retention rates. Through the study, I have created a clustering model with Silhouette Score at 65% that segregated customers into 2 clusters.


## Background

Insurance industry is highly commoditized and customer engagement is both limited and superficial.  Insurance companies have difficulty building a strong relationship with customers and maintaining customer engagement outside a claim or a renewal. For insurance companies to provide a superior customer experience that translates to customer retention, insurance companies must fully understand who their customers are, such as what motivates them, what concerns them, their hopes, their expectations and their life situations. 

Market segmentation will help insurance companies to improve customer experience and increase customer retention rates. By applying market segmentation strategy, all customers are divided into smaller sub-groups with one or more similar characteristics. This strategy helps insurance companies in <br>
(1) identifying specific marketable segments, allowing insurance companies to use different strategies to push renewals and upsells; <br>
(2) discovering untapped and profitable customer segments; and <br>
(3) identifying market trends that are not obvious and find ways of effectively meeting demand ([source](https://www.hyperon.io/blog/why-insurance-companies-need-customer-segmentation)). <br>

With market segmentation, insurance companies will be able to avoid head on competition in the market place by differentiating their offerings, not only on the basis of price but also through styling, packaging, promotional appeal, method of distribution and superior service ([source](https://nairaproject.com/projects/2110.html)). This in turn translates to high-value experiences and customer loyalty with satisfied customers remaining longer, renewing at higher prices, and recommending businesses to friends and family.


## Problem Statement

Insurance industry is overcrowded and competitive. Generally, customers can’t tell insurance companies apart and make decisions based on price alone. Hence, this causes insurance companies to disproportionately focus on price. As a result, insurance companies prioritize cost management, which reduces the quality of customer services and increases customer churn ([source](https://www.hyperon.io/blog/why-insurance-companies-need-customer-segmentation)).

In this project, I am tasked to develop a model that segregates customers so as to help insurance companies creating relevant offers that provide high-value experiences to customers that translates to increase in customer retention rates.
The model is expected to segragte customers into clusters. Metric used to assess model's accuracy in segregation is  Silhouette Score, which is used to calculate the goodness of a clustering technique. Its value ranges from `-1` to `1` ([source](https://towardsdatascience.com/silhouette-coefficient-validating-clustering-techniques-e976bb81d10c)).

`1`: Means clusters are well apart from each other and clearly distinguished. <br>
`0`: Means clusters are indifferent, or we can say that the distance between clusters is not significant.<br>
`-1`: Means clusters are assigned in the wrong way.<br>

Model is expected to achieve at least 50% in  Silhouette Score.


## Datasets

Dataset, which is provided by Prudential Life Insurance U.S.A, is obtained from [Kaggle](https://www.kaggle.com/competitions/prudential-life-insurance-assessment/data). 

| Data Type | Variable
|:---|:---
|Categorical|`Product_Info_1`, `Product_Info_2`, `Product_Info_3`, `Product_Info_5`, `Product_Info_6`, `Product_Info_7`, `Employment_Info_2`, `Employment_Info_3`, `Employment_Info_5`, `InsuredInfo_1`, `InsuredInfo_2`, `InsuredInfo_3`, `InsuredInfo_4`, `InsuredInfo_5`, `InsuredInfo_6`, `InsuredInfo_7`, `Insurance_History_1`, `Insurance_History_2`, `Insurance_History_3`, `Insurance_History_4`, `Insurance_History_7`, `Insurance_History_8`, `Insurance_History_9`, `Family_Hist_1`, `Medical_History_2`, `Medical_History_3`, `Medical_History_4`, `Medical_History_5`, `Medical_History_6`, `Medical_History_7`, `Medical_History_8`, `Medical_History_9`, `Medical_History_11`, `Medical_History_12`, `Medical_History_13`, `Medical_History_14`, `Medical_History_16`, `Medical_History_17`, `Medical_History_18`, `Medical_History_19`, `Medical_History_20`, `Medical_History_21`, `Medical_History_22`, `Medical_History_23`, `Medical_History_25`, `Medical_History_26`, `Medical_History_27`, `Medical_History_28`, `Medical_History_29`, `Medical_History_30`, `Medical_History_31`, `Medical_History_33`, `Medical_History_34`, `Medical_History_35`, `Medical_History_36`, `Medical_History_37`, `Medical_History_38`, `Medical_History_39`, `Medical_History_40`, `Medical_History_41`
|Continuous|`Product_Info_4`, `Ins_Age`, `Ht`, `Wt`, `BMI`, `Employment_Info_1`, `Employment_Info_4`, `Employment_Info_6`, `Insurance_History_5`, `Family_Hist_2`, `Family_Hist_3`, `Family_Hist_4`, `Family_Hist_5`
|Discrete|`Medical_History_1`, `Medical_History_10`, `Medical_History_15`, `Medical_History_24`, `Medical_History_32`, `Medical_Keyword_1-48`

#### Overview of technical analysis: 

(1) Problem_Statement <br>
(2) Understanding Data <br>
(3) Preprocessing <br>
(4) Modelling <br>
(5) Conclusion <br>
(6) Recommendations


### Conclusion
Customers are segregated into 2 clusters. Among all, cluster 0 has the highest count of data with cluster 1 having the lowest count of data.


### Recommendations
As the data has been normalized and dummified, it is challenging to derive meaningful insights from the data for product and campaign development for the targeted clusters. Hence, for future improvement, clarification could be seek from Prudential to understand the data and then to derive actionable insights; and to continue training the model with more data points.
