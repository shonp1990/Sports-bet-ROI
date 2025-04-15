# Optimizing ROI Across Bet Types in Sports Betting

Objective & Purpose:
I did this project purely because I have an interest in sports betting. I already use a sports betting tracking app that is synced to the 7 sportsbooks that I use but the app, while powerful and gives plenty of information, does not paint a full picture. With an interest in data analytics, I wanted to put my skills to use for a fun project where I can the most profitable bet types (Moneyline, Spread, Player Prop) in a one week span. 
About The Data:
The data comes from the sportsbooks that I use along with the tracking app called Pikkit which I used to go and find the odds that the bet was placed and what day. The data is from a 9-day period in February which I randomly chose to make the project a little simpler. I will list the fields below:
•	Bet_date
•	Bet
•	League
•	Bet_type
•	Odds
•	Risk_amount
•	To_win
•	Result
•	Net_profit
•	Roi
File type: CSV
Data structure: One Table
Total records: 72
Total fields: 10
Last Updated: 04/08/2025
Prepare & Import/Export Data in SQL:
1. Formatting – For SQL to properly identify the bet_date as a date, I had to convert the bet_date fields to the proper SQL date format (yyyy-mm-dd) before uploading to SQL.
2. SQL Importing – Created a new Schema (bets) in SQLite and imported the CSV file as a new table.
3. SQL Queries – In SQLite, I did five different queries to get a glimpse of my table.
•	ROI per Bet Type – I had 3 different bet types, moneyline, spread and player prop. Out of the 3 bet types, I bet on the spread a total of 43 times with an average ROI of -4.5581. 
 
This query allows me to see the total number of bets for each bet type along with getting a sense of how many wins and losses and total profit.

•	Win Rate per Bet Type – This query was for risk evaluation to tell me how often each bet type wins.
 

•	Average Risk and Payout per Type – Generally, I risk $5 per bet but during this particular week, I dabbled with different risk amounts. I find this query to be useful because I am always intrigued by how much I can potentially win.
 

•	ROI by Odds Range – I find this query to be the most useful because now I can see which odds range I am the most profitable in. This data is something I do not have access to in my bet tracking app.
 

•	ROI by League – This query was not needed for me personally because I already knew the results would not be to my liking, but I still thought it would be interesting to see what leagues, if any, returned a profit.
 
4. Exporting Results – I exported my query table results from SQL and brought my table into Tableau to visualize my findings.
Dashboard:
I created a dashboard in Tableau with 3 different charts:
•	ROI by Bet Type – I created a bar graph and calculated the average ROI for the bet types and added filters to make the bar graph interactive.
•	Net Profit by League – I created a bar graph to show total profit for each league in the dataset. I also added filters and added a formula for dynamic colors for the bar graph.  
•	ROI by Odds Range – I created a bar graph to show total profits by odds range. Dynamic coloring and filters were also applied. 

 
Insights:
1.	Best performing League – If we go off the charts and SQL queries, the best performing league would be Tennis but the sample size is too small to justify further action. I think what I can take from this is to put more action towards +100 to +199 odds going forward.
2.	Poor Performing Category – Player Props is the obvious red flag but there was one bet that is considered a longshot (over +200) that did not win and impacted the results in a bad way. Once again, the sample size is small so it is still too early to say that I should avoid player props altogether.
3.	Most Profitable Odds Range – According to the chart, my most profitable odds range was +100 to +199. I think with this data, I can double down on bets between these odds range. In contrast, I should be cautious when it comes to odds that are -111 and lower.
Conclusion:
Not the results I wanted as far as profit but knowing where I succeed and where I should stay away from is what I wanted from this project. Going forward, I feel confident in taking more of a risk with certain odds and trying different approaches to the less performing odds.
