# Foreign-Exchange-price-prediction

## Introduction
The foreign exchange rate is the price of one currency in terms of another. Because the foreign
exchange rate compares the currencies of 2 countries, the rate depends on the value of each
currency and, thus, on the economies of both countries. There are 3 primary economic factors
that affect the foreign exchange rate:

1. the relative purchasing power of each currency;
2. the investment opportunities and risks of each country
3. the desirability of the goods and services of each country.

Although other factors can be enumerated, such as the international balance of payments, they
can all be subsumed under these 3 primary economic determiners of the foreign exchange rate.
Foreign Exchange rate is one of the most important means through which a country’s relative
level of economic health is determined. A country's foreign exchange rate provides a window to
its economic stability. It would be great if we could precisely predict how these rates will change
in the far or near future. There are a lot of factors affecting the movement of foreign exchange
rates that it is hard to model . It’s movement depends on several factors like inflation , interest
rate , political stability and economic performance of the country , terms of trade , public debts
and many more.Therefore, predicting stock prices is a difficult job, but we still have valuable
tools which can help us to understand the foreign exchange movement up to some point and in
this project we use Geometric Brownian Motion and Martingale to make these predictions.
The purpose of this project is to study the basic properties of Geometric Brownian Motion and
Martingale Process and make an application of the properties covered. We will use the
Geometric Brownian motion and Martingale Process to predict the Foreign Exchange Rates of
the following five countries : India , China , Japan , United Kingdom and Brazil and then analyze
the results obtained.


## Result
We have taken mean absolute error as the metric for the model accuracy and analysed the results
for five highest countries in terms of GDP India,China,UK,Japan and Brazil. Focus was to
analyse the policy which have led to such trends and if any one of the models can be used for
their exchange rates prediction. Table 1 shows the accuracy for each country on different models
and thus the prediction depends on the policies of each country and inflow outflow of
investments in the country . Results for each country are discussed in the subsections.


<img title="Table 1. Mean Absolute Error for different models" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/MAE.png" />

### India

<img title="Fig 3. Foreign Exchange Trends of Indian Rupee(2000-2020)" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/indian_trends.png" />
<img title="Fig 4. Geometric Brownian Motion Prediction on Indian Rupee Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/gbm%20india.png" />

<img title="Fig 5. Martingale Prediction on Indian Rupee Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/mp%20india.png" />

In the 19th century, large increases in the quantity of silver production caused a precipitous drop in silver's value, leading to a steep decline in the rupee's value. From 1927 to 1946, the rupee was pegged to the British pound. It was then pegged to the U.S. dollar until 1975. India has been losing its investments and thus we can see that in fig 3.  that  the rupee is becoming weak in comparison to usd. GBM in fig 4. Predicts the rates with a mean absolute error(MAE) 0.4351 whereas Martingale in fig53. predicts the rates with MAE 0.319 . Therefore the differences are not significant and we know that both the models can help us to accurately predict the prices.


### China

<img title="Fig 6. Foreign Exchange Trends of Chinese Yuan(2000-2020)" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/china_trends.png" />
<img title="Fig 7. Geometric Brownian Motion Prediction on Chinese Yuan Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/gbm_china.png" />

<img title="Fig 8. Martingale Prediction on Chinese Yuan Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/mp_china.png" />


The USDCNY exchange rate is a reference rate not used in actual currency trading. When investors or entities want to exchange dollars for the Chinese currency, they do so using the USD CNH exchange rate set in Hong Kong.As from the past 20 years trend we can observe that china was indulged in currency pegging (since 1994) i.e it controls it foreign exchange rates to make the chinese exports cheaper and moreover the prediction both through GBM and Martingale can’t be relied on as they prices will be kept on pegged by the Government of the china but if the case would have been any different the GBM and Martingale have MAE of 0.102 and 0.109 respectively although the difference doesn’t seems to be significant but the the changes in chinese exchange rates are also not significant  so MAE doesn’t shows the clear picture.

### Japan 

<img title="Fig 9. Foreign Exchange Trends of Japanese Yen(2000-2020)" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/japan_trends.png" />
<img title="Fig 10. Geometric Brownian Motion Prediction on Japanese Yen Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/gbm_japan.png" />

<img title="Fig 11. Martingale Prediction on Japanese Yen Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/mp_japan.png" />

The Japanese yen has see-sawed in the last 35 years, particularly in the first decade after the 1985 Plaza Accord, in which a deal was made to devalue the U.S. dollar, therefore strengthening the yen and this pattern is completely visible from the exchange rate graph in fig 9, from the GBM prediction majority of the predictions have been stable around the price of 102-120 and at current it s conversion rate is 104.66 Yen=1 USD which shows that GBM can be more reliable for prediction than Martingale as the MAE for GBM is 0.55 whereas for Martingale MAE is 1.94 which shows a significant difference.

### United Kingdom

<img title="Fig 12. Foreign Exchange Trends of UK Pound(2000-2020)" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/uk_trends.png" />
<img title="Fig 13. Geometric Brownian Motion Prediction on UK Pound Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/gbm_uk.png" />

<img title="Fig 14. Martingale Prediction on UK Pound Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/mp_uk.png" />


The British pound has one of the highest trading volumes in the world, trailing only the U.S. dollar, euro, and Japanese yen in daily volume. The British pound accounts for roughly 13% of the daily trading volume in foreign exchange markets. The pound symbol is £.The British pound is the oldest currency in the world that is still used as legal tender. During the referendum of 2016 the UK policy on brexit likely makes us see that the pound became weak as compared to the USD , unlike the previous  analysis the Martingale does not show a lot of randomness and shocks in the predictions as compared to the GBM predictions but Martingale shows a slight probability of Pound strengthening and so the GBM .The mean absolute error using GBM is 0.039 and using martingale is 0.041 the difference is not significant and thus both the models can equally produce effective results.

### Brazil

<img title="Fig 15. Foreign Exchange Trends of Real(2000-2020)" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/brazil_trends.png" />
<img title="Fig 16. Geometric Brownian Motion Prediction on Real Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/gbm_brazil.png" />

<img title="Fig 17. Martingale Prediction on Real Foreign Exchange Rates" src="https://github.com/NishantSushmakar/Foreign-Exchange-price-prediction/blob/main/Image/mp_brazil.png" />

The British pound has one of the highest trading volumes in the world, trailing only the U.S. dollar, euro, and Japanese yen in daily volume. The British pound accounts for roughly 13% of the daily trading volume in foreign exchange markets. The pound symbol is £.The British pound is the oldest currency in the world that is still used as legal tender. During the referendum of 2016 the UK policy on brexit likely makes us see that the pound became weak as compared to the USD , unlike the previous  analysis the Martingale does not show a lot of randomness and shocks in the predictions as compared to the GBM predictions but Martingale shows a slight probability of Pound strengthening and so the GBM .The mean absolute error using GBM is 0.039 and using martingale is 0.041 the difference is not significant and thus both the models can equally produce effective results.

## Dataset 
 
https://www.kaggle.com/brunotly/foreign-exchange-rates-per-dollar-20002019
