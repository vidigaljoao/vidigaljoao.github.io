---
layout: posts
title:  "Data Visualization - Stock Prediction Dashboard"
date:   2019-08-25 08:33:25 +0200
author: "João Vidigal"
tags: [data science, Visualization]
excerpt: "Visualization"
---

"A picture is worth a thousand words" 

Why do we create visualizations? 
There are many answers to this question but in my view they all come together with two ideas, discover and delivery.

Discover is finding ways to process and calculate the data, how to reason about it or even see it in a context. Then we have Delivery, how we define and share information. An import tool if you want to present an argument or convey information.
Visualization is communication, and is an integral part of the business value of a company.

Data visualization can be a simple plot or a complex dashboard. 
Dashboards take visualization to the next level by updating  according to data modifications. Also, dashboards enable easier comparisons between different models. Data scientists spend the majority of their time cleaning and wrangling data so they can extract valuable insights. Dashboards have the added benefit of helping in that aspect. Also, they can help other users that were not behind the code to play and filter the data.

Three major components compose this dashboard architecture:

* 1. **Data Collection**- First we collect the Yahoo financial data using the yahoofinancials library . Then we need to clean and wrangle the data so the model can use it .

* 2. **Forecast Model** using Facebook forecast library. To predict the value of stocks in the next days we used the prophet, an easy and robust forecast model built to aid in business time series problems. To measure model performance we used  the root-mean-square error (RMSE). 

* 3. **Dashboard Layout** built using the new pyviz library to construct dashboards, Panel . The dashboard enables interactive visualization and parameter change. It gives a big picture of stock time series and the forecast model. 