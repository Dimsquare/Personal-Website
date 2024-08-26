---
type: ProjectLayout
title: Machine Learning Model making Predictions on the GBP/USD exchange rate
colors: colors-a
date: '2024-01-15'
client: Relevant
description: >-
  I undertook a project to create a machine learning model which made
  predictions on the GBP/USD exchange rate using a classification algorithm.
featuredImage:
  type: ImageBlock
  url: /images/Screen Shot 2024-01-26 at 12.56.07 AM.png
  altText: Project thumbnail image
media:
  type: ImageBlock
  url: /images/bg2.jpg
  altText: Project image
---
Methodology

            For the purpose of this artifact, I decided to create my own machine learning model using accurate daily data on the GBP/USD exchange rate and python libraries such as pandas, sklearn and matplotlib in order to build the model and visualize the data I was using. The method I was using and the fact my project relied on the forex market made my project lack a lot of flexibility as it is difficult to locate accurate sources of data. Furthermore, due to this lack of accuracy and wholeness of the data, data cleaning became a tedious process. 

Figure 1:

![](blob:https://create.netlify.com/f7ee3903-6ac0-48ad-b688-e2682422c243)

\<div style="text-align: center">*Figure 1 represents the original values of the Forex Market*\</div>

During the training of this model, multiple variables were used to produce this machine learning model such as a new column called “Tomorrow” which represents the value of the exchange rate on the next day in order to make comparisons so that the model can learn. The results of this comparison were then stored in the column “Target” which shows whether the market went up or down indicating whether or not the individual should invest based on the past data. These were included in the data preprocessing and cleaning stages of the model. During the training stage of the model, variables such as “train” and “test” were used to actually train and provide the avenue for the model to learn and predict the stock market. These values were stored in a new variable. Utilizing the [pandas]() library, I was able to display the accuracy of my machine learning model.

Figure 2:

![](blob:https://create.netlify.com/5d508cfa-6896-4769-86ba-528298b92b3e)

\<div style="text-align: center">*Figure 2 represents the Forex Market after the learning parameters have been added.*\</div>

 

 

Data Collection and Preprocessing:

            In order to acquire data on the forex market, I made use of Alpha Vantage, which is generally regarded as a reliable source of financial information. “Alpha Vantage is a free source for financial data that in many cases is more accurate than Yahoo Finance and Google Finance” (The Comprehensive R Archive Network, 2023). This source can be deemed reliable as R is known to be the best programming language and source when it pertains to statistical and financial data. Furthermore, the data on the Alpha Vantage library is updated daily, increasing the accuracy and reliability of this python library. Additionally, Alpha Vantage provides data from up to 20 years ago which is updated daily to improve the accuracy of the model. During the importing of the dataset, I encountered one major setback. I was not able to import the dataset on a regular Python IDE (Integrated Development Environment) which delayed my progress for a week trying to debug and find out the problem with my program. I eventually realized I needed to use an IDE known as Jupyter Notebook rather than Visual Studio Code in order to actually import this dataset which further reduces the flexibility of this program. When importing the dataset and introducing the “Tomorrow” variable, data cleaning and normalization was severely needed as various columns has “NaN” as their values, which would disrupt the flow of data and the result of the model. In order to eliminate this disruption, any column with this value was eliminated which reduced the amount of data to work with from 5000 to 4000. During the data processing, the most influential columns became the “Open” column which represents the value of the currency when the market opens, the “Tomorrow” column which represents the value of the currency when the market opens the next day and the “Target” column which indicates whether the market went up and down.

Results and Analysis

            The results of the machine learning model resulted in an average 57.2% accuracy rate over a period of two days.

![](blob:https://create.netlify.com/bc024236-e9bf-4dd5-8b2c-27f782615892)*
Day 1 results*

![](blob:https://create.netlify.com/0211a629-e5aa-47df-94da-1efcb595a335)*
Day 2 Results*

![](blob:https://create.netlify.com/58c060ce-f011-4cfb-8abd-a05f2fbe9179)
The last diagram represents the modifications I made to the model in order to make it more accurate which resulted in an increase of 1% in accuracy. The new model was an improvement over the initial model because of a concept known as backtesting. “Backtesting in machine learning is a technique used to evaluate the performance and effectiveness of a machine learning model using historical data. It involves testing the model on past data to simulate how it would have performed if it had been used to make predictions during that period” (Zaidi, 2023). This improved the model because instead of directly trying to predict the exchange market in the near future, it makes predictions on the foreign exchange market on a known date, with a known value and adjusts to this known value accordingly.

Additionally, I tried to take other factors into account such as trying to use the close ratio and non-financial factors into account but realized getting access to high quality and accurate data on the economic state of the countries will be difficult and time consuming. These changes to the model resulted in a reduction of its accuracy by 20%.

![](blob:https://create.netlify.com/e4dec102-5bb0-4462-b504-76a248a7485a)

\<div style="text-align: center">*Model after non-economic factors taken into consideration.*\</div>

            These results have a significant impact as it really highlights the importance of having accurate and significant amounts of resources available in order to make an effective model. The fact that non-financial factors could not be taken into account in this model due to its inaccuracy shows that this model can be improved by up to 30%. This can be proven due to the research carried out by ThuongMai university which was referenced earlier. Despite the fact that they used EUR/USD which may have affected the accuracy of the results, both GBP and EUR have faced similar non-financial issues which may have an effect on the model. Hence, the model can significantly be improved along these lines.
