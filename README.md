# Do-stocks-go-to-one
In this project, I am trying to emperically test the popular saying "stocks go to 1", or that stocks tend to perfectly corelate during times of crisis (bear markets) with each other. I'll extend this saying to test the correlation with the market and even the correlation of the betas during crises. 

# Set up
I first create a percentage return in index returns. We use the S&P 500 index for the data. We take the data from 1980 to 2023. I prefer using the dataframe due to a lot of the current major stocks in the S&P 500 only start from the late 70s (Apple, MSFT etc). We Assume that the initial stage is bull market because we want to measure from the first drop in 20% from base. Using our definition of bear market phases, we find 8 bear markets. We find that there is the largest expansion from 1987 to 2001. The latest bear market was in 2022, the tech market crash. 
![image](https://github.com/user-attachments/assets/c31ca077-1cf5-4aec-8e30-44bbc9de4c1d)

Below we can see the bear market periods highlighted
![image](https://github.com/user-attachments/assets/fdf3edde-d70c-440b-91f1-bfe890591620)

In this graph, we can see that the largest bear market was in 2022. The shortest was in 2020, during the covid pandemic panic.

![image](https://github.com/user-attachments/assets/4defa6ab-2491-4d37-bee1-780a9f26955f)

In the above, we have measured the intensity of the bear markets to the investors. The 2022 bear market, which saw the tech crash still saw 10% returns on the market index. This could be due to the crash mainly affecting tech sector. The worst bear market was in 2008, coinciding with the housing bubble crash. This means that the market was broadly affected.

# Stock Correlation Findings
1. Correlation with the market
![image](https://github.com/user-attachments/assets/e49db29c-2a8b-411e-8d7f-5965f9bded82)

In the above, we have made correlation of the stocks against the index during the bear markets. We can see that only in a few of the phases, the stocks on average tend to 1. Otherwise, they are near 0.8. The highest correlation to 1 was in 2020. This maybe because the Pandemic affected the entire market.

2. Pairwise correlation - during the bear market
![image](https://github.com/user-attachments/assets/54e9943b-0bd2-4dd4-b4d0-7e2b3d34da8b)

In the above, we have calculated the average of piecewise correlation among all the stocks only across the different phases. In the graph we can see the average piecewise correlation in bear markets was 0.7 in the 2020 crash, one which affected every firm equally. Otherwise, correlations are not close to 1.

3. Pairwise correlation - monthly throughout the years
![image](https://github.com/user-attachments/assets/d797b388-6db8-4ecf-9b93-bbf9966934c3)

In the above, we have measured the average piecewise correlations each month from 1980 to 2023. Even this graph, shows that the average correlation is not remotely close to 1. The highest being during 2020 crash.

Therefore, from the above findings, we can say that correlation goes to one during crisis is not empirically supported by any type of test.

# CAPM Beta correlations

![image](https://github.com/user-attachments/assets/afe36c8f-ccdb-4d41-b621-7bdbdb80179f)

From the above, we can see that the average beta of all stocks is from 0.72 to 1.1 during any of these crises. There is high volatility in all crises, with the worst during the housing crash. The least beta is -1.01 during the 1987 crash and the highest beta is 5.89 during the tech bubble 2002 crash.

![image](https://github.com/user-attachments/assets/61d504ce-05e7-4466-bdcd-9e0298d60d16)

From the above density plot we can see that on average beta in the market is centered around 1, during all the crises, with the highest being in 2002 and 2020.

Therefore, from the above, we can conclude that CAPM Beta goes to 1 during crises is more empirically supported. We can make more studies into this.

