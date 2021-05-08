# Surfs Up

Background

My business plan is to set up a 'Surf and Shake' shop in Hawaii around the Oahu island. I've reached out to an investor called W.Avy for financial backing. To get W.Avy and his board of directors on board with this business venture, he has some weather concerns that need to be addressed and requires some data analysis to be done on some weather data sets. In this analysis, we will focus on the temperature trends to determine if the ice cream and surf shop is sustainable all year round using Python, Pandas, Matplotlib and SQLAlchemy.


-----

## Results


* December is a slightly cooler month than June. The average temperate for December is 71 degrees while in June it is closer to 75. That's roughly 4 degrees difference.
* In the IQR, we can see quite an even distribution in both months with December being on average 4 degrees lower across the IQR.
* The difference between December and June is mostly in the standard deviation where the spread is much higher in December. If you look at the minimum temperature for December it is significantly lower than in June. This has contributed to a higher standard deviation for December that is not captured in the IQR.

| June Summary Statistics    |  December Summary Statistics |
|---------------------------|---------------------------|
![june](https://github.com/YanLuong/surfs_up/blob/main/Screenshots/summary%20stats%20june.png) |![dec](https://github.com/YanLuong/surfs_up/blob/main/Screenshots/summary%20stats%20dec.png)
