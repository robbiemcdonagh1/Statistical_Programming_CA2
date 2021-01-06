# Statistical_Programming_CA2
C18772641 Statistical Programming CA2 6th January 2021 by Robert McDonagh 
This README file is to provide a breif explaination of the code provided in a little more deatil than the comments in the code provides. Initially we are required to import the necessary libraries to help all of our code run smoothly.

After that I imported the CSV files using tibble. I did this so that we can join our files together. The paths for csv files are unique to the user as every computer usesa different path with different names so be cautious of this.

Once i have my csv files loaded in it is important to check them to make sure there are no errors. Lines 16-20 are there to view the datasets. This allows us to see if there are any mistakes within the tables. Lines 23-27 check for any missing data values within the tables. If there were null values present it would alter our results so we must be cautious of them. I needed to make the files universally compatible, so I had to change a few  of the column names so I could join them with the final table. Once we have all the datasets are loaded under the correct variable names and there are no null values then we are ready to start using them for analysis.

Arounf line 32 we begin to set op  our tallys. The function of these is to count the number of times a specific variable appears in a column. I used tally for all of our impressions, clicks and conversions . These numbers were small but if we used a bigger dataset the results would be much clearer. I had to change the column names, such as "NoOfClicks".

Once i had my data in a useable format i needed to join it all together in a useble format. I used the inner join function to complete this. Inner Joincreates a new table by combining rows that have matching values. We had to edit some of our column names to ensure they had matching values to continue. inner_join was used to connect all our tallys using the keys created by changing column names. These inner_joins create the ad_data that I was able to use for the graphs to try and visualise how affective the ad campaigns were. This ad_data contains the names of the advertisers, the campaigns , their Budgets and the amount of impressions,clicks and conversions.












