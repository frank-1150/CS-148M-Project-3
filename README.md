# CS-148M-Project-3
The final project for UCLA course CS 148M 2021 Fall. We

1) build a predictive model for sales by brand using the given sales dataset with a R^2 score of 0.993; 

2) find 2 key indicators for successful product using Bayes theorem

## Files
- first discussion.pbix is the PowerBI dashboard we built for analysis
- CS148 Project 3 Fall21.docx.pdf is the problem statement
- Report v2.0.pdf is our final report

## Project background

Cookies was founded in 2012 by Gilbert Anthony Milam Jr., better known by his stage name Berner,and
his partner Jigga, Bay Area cultivator and breeder.  The cofounder leveraged a unique confluence of
emergent genetic engineering, internet culture, and strong associations with the music industry, to 
beone of the first companies to establish an identity and streetwear company that has come to 
dominatethe industry.

Today, Cookies is one of the most respected and top-selling cannabis brands in California and is 
globally recognized, amassing a stable of over 50 cannabis varieties and product lines including indoor, 
outdoor and sungrown flower, pre-rolls, gel caps and vape carts.  With two flagship Cookies stores in Los 
Angeles on Melrose and Maywood and a third location in Redding, Cookies' overall vertical integration and 
seed to sale business allows for complete quality control at every step from cultivation and production 
to retail experience.

In 2015, the brand's hip-hop credibility effortlessly expanded Cookies into streetwear and today 
offers a range of products for both men and women in the apparel and accessories categories as well as a
curated selection of smoking supplies

## Our method
### Part A: Predictive model for sales by brand

We built two features on sales (sales in previous month and rolling average of 3-Month sales), one feature about the brand (Category L1), and extract the time information by creating three time-related features: year, month, quarter. We then construct three models (Linear Regression, Random Forest and XGBoost model) to run test on. The result is that our best model, XGBoost does well in predicting the sales of big brand (monthly total sales>500,000) and medium brand (monthly total sales<500,000 and >10,000) with a R2 score of 0.993 and 0.786 respectively.

### Part B: Finding key indicators for successful product

We build two metrics to measure how good a certain category of product sales in the market: market share score and out performance score. Market share score shows the empirical probability a certain product that a certain product's sales will rank in the top third of the market. Out performance score shows how much a certain indicator can affect the market share score. After traversing all possible values for all the features given in the dataset, we find that the “Flower” in Category L2 and “Hybrid” in Category L3 is the best sales-prompt indicators. 

This result tells us that picking a growing, less-competitive niche market, is the key to grow revenue in the cannabis industry.

## Some Buisiness intelligence graphs
 ![image](https://user-images.githubusercontent.com/76094159/208984086-414e468d-7af9-4e91-b318-948bd80ccf67.png)

Total Sales of the whole market rises from 40 million to around 55 million per month.

![image](https://user-images.githubusercontent.com/76094159/208984142-f7810e82-7729-46c1-8a2f-e8bbf6a0afcf.png)
Comparing the total sales Year-on-Year changes, we can see the strong growth in 2020 and the slowing down in mid-2021.

![image](https://user-images.githubusercontent.com/76094159/208984197-86701147-4a3c-4437-bd4e-faa5e2f91276.png)

![image](https://user-images.githubusercontent.com/76094159/208984215-5b3bc97d-15ab-4dbf-b988-99f03a10abb3.png)

![image](https://user-images.githubusercontent.com/76094159/208984231-0c6fa71a-0b14-46d6-8052-6d5d4cd4987b.png)

![image](https://user-images.githubusercontent.com/76094159/208984030-30f7c527-0acc-4433-8f93-f428c2bb3420.png)


