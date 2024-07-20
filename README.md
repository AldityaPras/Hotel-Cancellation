# **HOTEL CANCELATION'S PREDICTIONS**

Made by : Muhammad Alditya Prasetyawan
Class   : DTI-DS 0106

**Table of Content**
1. Business Problem Understanding
2. Data Understanding

<br>

## **Business Understanding**

#### **Context**
Portugal, renowned for its rich history dating back to the medieval era, is celebrated for its remarkable architecture, distinguished naval history, and significant Catholic heritage sites. The country's allure naturally attracts numerous tourists, contributing to a thriving hotel industry. To support the robust tourism sector, effective management of the hotel industry is crucial. Based on [Revfine](https://www.revfine.com/tourism-industry/), hotel industry is included in top 3 sector that support tourism.

#### **Problem Statement**
Hotel industry normally has numerous challenges and one of them is customer booking's cancellation. This cancellation booking might cripples the hotel industry, especially in operational sector, therefore it is vital to determine operational cost [Article](https://shrgroup.com/2023/06/21/we-need-to-talk-about-cancellations/#:~:text=Now%20in%202022%2C%20our%20latest,2019%20for%20the%20same%20period). Moreover, Based on the findings, one of the main unnecessary cost loss is because of food spending[Article](https://www.hospitalitynet.org/opinion/4112912.html).

#### **Project Stakeholders**
The stakeholders who will utilize this model include:

* Operational Department: This department will handle the food supply, run the food operations and manage food storage. Therefore, they require specific calculation and budget for food operations.
* Finance Department: One of the Finance Department's tasks is to manage the company's income and expenses, which include the costs incurred from customer needs (ex. breakfast, fixed cost, etc).

#### **Project Goals**
The main goal here is to create an effective classification model. This model's job is to predict the limit of hotel expenditure on food and calculate the potential revenue of food distribution strategy. It's important that this model is good at predicting customers that will cancel the booking. This strategy will help the hotel to use their resources better, make their interactions with customer more effective, get better rating and ultimately, generating more sustainable revenue.

#### **Metric Evaluation:**
This analysis will focus on customers cancellations. The targets are defined as follows:

* 0: indicates a customer who does not cancel the booking.
* 1: represents a customer who does cancel the booking.

Ensuring the accuracy of our model is crucial to avoid the financial repercussions of misclassification, which could come in the `form of False Positive or False Negatives`.

| **Error Type**     |**Explanation** | **Consequences** | 
|-----------------|------------|----------------|
| **False Positive / Type 1 Error**  |A situation where customers are predicted to **cancel** their bookings but, in reality, do not cancel them.| Average food cost in Portugal is [8 EUR](https://authentik.com/be-en/destinations/portugal/faq/calculate-food-budget). If The food cost calculation is not effectively targeted, resulting in excess loss. Without machine learning models it will create `financial loss up to 10 EUR`. |
| **False Negative / Type 2 Error**  | A situation where customers are predicted not to cancel their bookings but, in reality, do cancel them.| The hotel loses potential customers, which results in lost revenue. Therefore, in the worst case, the hotel earns `90 EUR after deducting 8 EUR food costs`.| 

<br>
