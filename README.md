# USpolice-EDA

This code analyzes data on fatal police shootings in the United States using three datasets: police_shootings, population, and kaggle_share_race.

First, the code imports the datasets using pandas and prints the first few rows of each dataset using the head() method.

Next, the code merges the police_shootings and population datasets into a new dataframe called merged_df using the merge() method from the Pandas library. The merge is performed using the city and state columns as the join keys. The how='left' parameter specifies that all records from the police_shootings dataset should be included in the merged dataframe, even if there is no matching record in the population dataset. The resulting dataframe merged_df contains all columns from both datasets, and any missing values are filled with NaN.

Then, the code creates a histogram using Seaborn to show the distribution of ages among the people killed in police shootings. The merged_df dataset is used as the data source. The histogram is created using the sns.histplot() function, which takes in the data to plot and the number of bins to use for the histogram.

Finally, the code creates a count plot using Seaborn to show the distribution of races among the people killed in police shootings. The merged_df dataset is used as the data source.

The resulting plots show that the majority of people killed in police shootings are white, with over 3500 recorded cases. Black and Hispanic individuals are the next largest groups, with approximately 2000 and 1300 recorded cases respectively. Additionally, the majority of people killed in police shootings were under the age of 50, with a peak at around 25 years old.

It is important to note that this dataset is limited in its scope, as it only includes fatal police shootings and may not be representative of all instances of police use of force. Nonetheless, the disproportionate number of people from racial and ethnic minority groups who are killed by police has been a subject of concern and controversy, and efforts to address these disparities and promote police accountability and reform continue to be important.
