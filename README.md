# Surfs Up

### 1. Purpose and background

My business plan is to set up a 'Surf and Shake' shop in Hawaii around the Oahu island so that I may live there forever. I've reached out to an investor called W.Avy for financial backing. To get W.Avy and his board of directors on board with this business venture, he has some weather concerns that need to be addressed and requires some data analysis to be done on some weather data sets. In this analysis, the focus will be on temperature trends (June and December) to determine if the ice cream and surf shop is sustainable all year round using Python, Pandas, Matplotlib and SQLAlchemy. 


-----

### 2. Results


* December is a slightly cooler month than June. The average temperate for December is 71 degrees while in June it is closer to 75. That's roughly 4 degrees difference.
* In the IQR, we can see quite an even distribution in both months with December being on average 4 degrees lower across the IQR and summary statistics than in June.
* The difference between December and June is mostly in the standard deviation where the spread is much higher in December at 3.7 compared to June with 3.2. If you look at the minimum temperature for December it is significantly lower than in June. This has contributed to a higher standard deviation for December that is not captured in the IQR.

| June Summary Statistics    |  December Summary Statistics |
|---------------------------|---------------------------|
![june](https://github.com/YanLuong/surfs_up/blob/main/Screenshots/summary%20stats%20june.png) |![dec](https://github.com/YanLuong/surfs_up/blob/main/Screenshots/summary%20stats%20dec.png)


---

### 3. Summary

When comparing June and December, there is on average 4 degrees difference between the two months and it's a very consistent trend in the summary statistics. The difference lies in the standard deviation and the minimum temperature for December. The month of December has a much higher standard deviation than in June and this can be seen in the box plot below with the longer whiskers and significantly higher number of outliers. Below the minimum temperature for December, there are significantly more outliers than in June. This will impact and distort the summary statistics for December and drag down the mean and the IQR temperature numbers.
The first recommendation would be to address the outliers as it is currently distorting the temperature numbers for December. First step, would be to determine if the outliers are relevant(random events) or done in error? Since we know there are different stations that record the temperatures, we can filter out by station to get the minimum, maximum and mean temperatures for each station. If the results are consistent across all the stations then we can eliminate the idea that a station may have recorded some of the temperatures in error. Another way to identify if the outliers are specific to a station or not would be to plot a muitple line chart, with each line representing a station of the temperature recorded vs date on the same chart. This will provide a good overview of the temperature trends across all the stations over a period of time. The second recommendation would be to plot all the temperatures vs date on a scatter plot so we can see exactly when or where the outliers occured. Depending on the visualised results, it may be better to just remove the outliers to get a clearer picture of the results for December. And lastly, I would recommend running the same analysis for each month. That way we can observe the general temperature stats for the whole year.

![box plot](https://github.com/YanLuong/surfs_up/blob/main/Screenshots/combined%20box%20plot.png)
