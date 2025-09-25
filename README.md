# Stock-Prediction-Model

## Predicting Stock Price Movement using LSTMs:
Predicting Microsoft(MSFT) stock price movement based on the daily closing price. Creating a custom LSTM model, and training it based on a window of past 3 working days. Thereafter checking for which intervals the model works and figuring out the reasoning behind it.

## Dataset: 
The dataset is obtained from yfinance and a link to the same can be obtained [here](https://finance.yahoo.com/quote/MSFT/history/?period1=511108200&period2=1718603577).

## Model: 
The model is a custom LSTM network, that was chosen because of LSTM networks' ability to make predictions based on previous data. The model was trained by providing the past 3 business days' closing price as input with the next days closing price as output. The model was trained twice, once on long term all time data and once on a short term data dating back to 3 years only.

## Discussions: 
The model seem to perform better on short term data than long term data. It can keep up with the small changes of the market but is unable to predict sudden large changes in the market. Following are some pictures of long term and short term: 

### Long Term- 
![Recursive Long Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/33ff5da8-35e1-4ffb-8b20-754c2c4ea82a)
![Testing Long Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/5024259e-64c5-4b80-84a7-9e16273cde94)
![Everything Long Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/9afb41d2-c5c1-4831-8061-f6cec6d97572)
![Validation Long Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/9adc0fb9-31ac-4968-8e8b-ca0757c39993)
![Training Long Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/fea329eb-2176-4145-8685-dc4d172e1770)

### Short Term-
![TrTeSp Short Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/c3fd9fb0-f8ce-4640-bc04-231af177f7c5)
![Short Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/9b73ba75-447a-4d74-a7a3-b44065c1019d)
![Validation Short Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/24247053-a941-4e28-9736-8f361e626bee)
![Testing Short Term](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/21bd3c47-729a-4876-9b64-4575409bebfa)
![Short Term 2](https://github.com/avanishgadhikar/Stock-Prediction-Model/assets/133745149/3b6c808c-8149-4a9d-9080-dbbeea240353)


## Results:
We can see here that the minute there is a big change as seen in the rise of stock in 2023-Nov, the model is unable to predict it and thus fails to predict that data, but if the change is not much, the model can track it pretty well. We can see how it is unable to predict the volatility in the stock prices, and thus its uses are solely limited to this learning based project.
