# Ed-Foote-Project-2
## SMA and MACD Signals in a Algorithmic Trading Model 

## Required imports:

Pandas, NumPy, hvplot, matplotlib, pyEX, sklearn, yfinance

## Data Source
We pulled our data using an API from Yahoo Finance 

## Project Overview:

Our goal was to analyze various signals and assess whether a simple maachine learning model could predict the trading strategy. 
We focused on the Simple Moving Average and the Moving Average Convergence Divergence. 
Both SVM and Logistic Regression models were used to assess model accuracy. 


## JPM MACD
<img width="310" alt="JPM MACD" src="https://user-images.githubusercontent.com/86026996/139519905-38f7118a-7417-4503-9def-4c9584195a1a.png">

### MACD SVM Classification Reports 
<img width="380" alt="Screen Shot 2021-10-29 at 11 23 22 PM" src="https://user-images.githubusercontent.com/86026996/139520009-b3717de6-dc62-4d4e-8915-91836259677a.png">

### MACD Logistic Regression Classification Reports 
<img width="399" alt="Screen Shot 2021-10-29 at 11 23 43 PM" src="https://user-images.githubusercontent.com/86026996/139520015-67e04821-0530-435b-a935-367d07af18bd.png">

The classification report has led us to conclude that our training model did not capture enough Buy and Sell data points relative to Holds.
Because there were so many Holds and so few Buy and Sells, the model was unable to accurately predict any points. Thus, if additional time 
was devoted to the project, alternative methods for aggregating testing data may be needed. Oversampling may be one solution. 



## JPM SMA 
<img width="307" alt="JPM SMA" src="https://user-images.githubusercontent.com/86026996/139519924-7c14574d-33d2-4bf2-b0f1-21fc63f0812f.png">

<img width="299" alt="Screen Shot 2021-10-29 at 11 20 03 PM" src="https://user-images.githubusercontent.com/86026996/139519939-5811ce1a-3111-4809-a8d9-3a5872d660b6.png">

### SMA SVM Classification Reports 
<img width="388" alt="Screen Shot 2021-10-29 at 11 24 58 PM" src="https://user-images.githubusercontent.com/86026996/139520050-790a0784-4b10-453d-97a6-f787f7c9333a.png">


### SMA Logistic Regression Classification Reports 

<img width="381" alt="Screen Shot 2021-10-29 at 11 25 09 PM" src="https://user-images.githubusercontent.com/86026996/139520054-2d732c46-2a2f-4d18-8874-35dd79219755.png">

The classification reports from the SMA model indicates that the machine learning model accurately predicated trading decisions half the time. With a weighted average of 51%, much more work would be needed before deploying the trading strategy in the real world. 

