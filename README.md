# Surfs_Up

## Overview of the Analysis

The purpose of the analysis was to examine the temperature data for June and December in Oahu and determine whether the surf and ice cream shop business is sustainable year-round.

## Results of the Analysis

<ul>
  <li>A query was created utilizing the FILTER and EXTRACT functions to extract any temperature whose corresponding date contained a 6 (for June) in the month column.  The extracted data was placed in a variable called "june_temps," converted to a list, and then converted to the following DataFrame:</li>

  ![June_temps_df](https://user-images.githubusercontent.com/94088129/163185727-0c4f1128-b4c5-4e9c-91f5-5b1065fb92cb.png)

  <li>For further clarification of the June temperature data, we use the DESCRIBE method to view the summary statistics of the data</li>
  
  
  ![June_temps_describe](https://user-images.githubusercontent.com/94088129/163187091-91f41cb5-3d91-4a91-aff3-9eb2cc52a94b.png)

  <li>A second, similar query was created utlizing the FILTER and EXTRACT functions to extract any temperature whose corresponding date contained a 12 in the month column, indicating the month of December.  The extracted data was then placed in a variable called "dec_temps," converted to a list, and then converted to the following DataFrame:</li>
  
  ![Dec_temps_df](https://user-images.githubusercontent.com/94088129/163187546-3aee0651-a50e-4dc1-83cc-fc524d014143.png)

  <li>For further clarification of the December temperature data, we use the DESCRIBE method to view the summary statistics of the data</li>
  
  ![Dec_temps_describe](https://user-images.githubusercontent.com/94088129/163188018-8172f83a-0d82-4abc-a655-b221249d8ef9.png)

</ul>

## Summary of the Analysis

Overall, the temperature difference between June and December is visible, but doesn't make an ice cream and surf shop unsustainable.  The mean temperature in June is approximately 75 degrees, while the mean temperature in December is about 71 degrees.  While the maximum temperatures are 85 and 83 degrees respectively, the true difference between the months is evident in the minimum temperature, which is 64 degrees in June but 56 degrees in December.  

To further our conclusions, I would propose two additional queries.  The first is the VALUE_COUNT function, which would show the amount of days for each temperature in our DataFrame.  This would assist in showing not only which temperatures are seen most often in their respective months, but also how few days are in the outlying temperatures.  The second query would be to visualize the data, which would mean importing another library to utilize the visualization function.  While the VALUE_COUNT function would order our temperatures in order of most occuring to least occuring, I would organize the x-axis of the plot with the temperatures in numerical order, and the y-axis would indicate the amounts.  This visualization would better illuminate where our days fall on the temperature scale.  You can also overlay the June and December plots to more clearly note the differences between the two months.
