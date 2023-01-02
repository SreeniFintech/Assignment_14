# Assignment_14: Algorithmic Trading Assignment


### 1. Conclusions about the performance of the baseline trading algorithm
Actual returns and Strategy Returns are close to each other showing the ML is giving close results. It means that the performance of the trading strategy is somewhat in line with the performance of the trades that were actually executed. It indicates that the trading strategy can be further calibrated to be  able to accurately predict the movements of the market.
![Baseline trading Plot](https://github.com/SreeniFintech/Assignment_14/blob/main/image1.png)

### 2. Tune training algorithm by adjusting the size of the training dataset
- Slice data into different periods viz 4 months: Slicing the data into 4 months and 6 months further distorts the chart between actual returns and strategy returns
![Increase training window to 4 months](https://github.com/SreeniFintech/Assignment_14/blob/main/image2.png)
- Increase or decrease the SMA window: Increasing the SMA Window to 10 months further improves the performance of the trading strategy where the actual returns and strategy returns move equally. 
![Increase SMA to  10 Periods](https://github.com/SreeniFintech/Assignment_14/blob/main/image3.png)

- Set of parameters to best improve the trading strategy
-- SMA short window set to 10 periods
-- SMA long window set to 100 periods
-- Training window set to 3 months

### 3. Evaluate a New Machine Learning Classifier
- Using logirithmic regression classifier - 
- The logistic regression model did not perform better than the SVM model although it had a higher accuracy score. However, the SVM model does a better job predicting profitable short opportunities, as evidenced by its higher recall score on the -1.0 class. Ultimately, which model is best may depend on which class we care most about predicting, as well as which has better overall economic returns compared to a long-only investment
![Logirithmic Regression Classifier](https://github.com/SreeniFintech/Assignment_14/blob/main/image4.png)
