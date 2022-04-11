# Surfs_Up

## Overview of the Analysis

The purpose of the analysis was to examine the temperature data for June and December in Oahu and determine whether the surf and ice cream shop business is sustainable year-round.

# Results of the Analysis

In order to obtain the temperature data for June and December, two separate queries had to be crafted: one that would extract any temperature whose corresponding date contained a 6 for June in the month column, and one that would extract any temperature whose corresponding data contained a 12 for December in the month column.  To do so, we used a the FILTER and EXTRACT function to filter the data by the conditions set forth and then extract that data from the data set to be placed in a varible called "june_temps" for the June data and "dec_temps" for the December data.  Those variables were then turned into their respective lists, and then a DataFrame was created from those lists.
