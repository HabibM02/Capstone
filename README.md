# Capstone
# Canadian Federal Election Trends
The aim of this capstone project to try to foresee and analyze any trends in future Canadian federal elections based on historical data. I have elected to work with the datasets from the last 8 federal election cycles; all available publicly via Elections Canada. These datasets provide the following for each riding across the country: a) the winning candidate and the associated party, b) total number of votes cast, c) number of votes cast for the winning candidate, among other attributes. 

# Initial Results and Code
For this part of the Capstone, I gathered the publicly available election data for each year from 2004 to 2025. Then I normalized the columns and headers, and cleaned the data to make them ready for analysis. 
Using, VS Code, I extracted the winning candidate names and their respective parties for each riding. After this step, I created a column to distringuish the number of votes recieved in each election year. Then, using pdconcat, I combined these extracted data all in one data frame to the visualizations for the following: a bar chart to show Total Votes by Party; a line graph to show Party Support Trends; and a bar chart to show the voter turnout by Year. 

# Classifications (Predictive Analytics)
At this step, I decided to design a regression model to do some predictive analytics. The model that I attempted to create was to predict Liberal Wins by creating a column. This was done by combining all the data analyzed thusfar. 
The results:
The Accuracy sore is 0.7154989 meaning the model predicted the outcome correctly 71.55% of the time. 
The Classification report shows that the model is better at predicting non-Liberal wins than it is at predicting Liberal wins. Class 0 is non-Liberal, class 1 is Liberal. 
Confusion Matrix: False negatives (83): These are Liberal wins that were wrongly predicted as non-Liberal.
False positives (51): Non-Liberal ridings predicted incorrectly as Liberal.
