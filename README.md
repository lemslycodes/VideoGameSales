# VideoGameSales
This is an analysis of video game sales and user/critic ratings from kaggle. 
I ran a multi-nominal regression to investigate critic scores effect on global sales, controlling for genre.  
The data was analyzed using an multinomial regression using Global sales as the
dependent variable. The first model measure only the relationship between Global Sales
and Critic Scores. A second model measured the relationship between Global sales by
controlling for User Count, User Scores, Critic Count, and Genre. Finally, the third model
measured the relationship between Global sales and Critic Scores, controlling for User
Count, User Scores, Critic Count, and Genre.

Table 1 offers a summary of statistics for Global sales, User Count, User Scores, Critic Count, and Genre. In total there are 6,747 observations. Global sales offer the most impressive numbers with an average of 5.46 Million. In order of average sales: North American has the highest average of 4.83, European sales (4.63M), Other sales (3.77M), and lastly Japan sales(1.41M). The standard deviation values for all variables except Japan sales are relatively low, this indicates the values are clustered close to the mean. This means 68% of Japan's sales were between 2.2 and 1.4 million dollars. It has more variance meaning some games sell well and some sell poorly. Our correlation matrix shows most of the variables have a moderate to weak linear relationship, the strongest positive relationship is between User Score and Critic Score (0.577) and our weakest positive relationship is between User Score and Critic Count (0.122).

