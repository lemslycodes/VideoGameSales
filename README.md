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

I used scatter plots to see if we can identify a relationship between the variables we are interested in. We see that there is a slight positive relationship between Critic Scores and Global Sales. Before I  actually do the linear regression, I will check for correlations between our two variables. The correlation between Global Sales and Critic Score is positive, statistically significant, and very large (p > .001). Due to the high correlation for both variables, we will also check for multicollinearity. 

In the first model, the bivariate relationship between Global Sales and Critic scores — an ordinal logistic regression was conducted using Global Sales as the dependent variable. The model explains a statistically significant and weak proportion of variance (P < 0.01). There is a positive correlation between Global sales and Critic Scores, 12.8% of global sales can be explained by critic scores. 

In the second model, I fitted a linear model to predict Global Sales with Critic Count, User Count, User Scores and Genre. I removed the independent variable to examine the relationship between the dependent and control variables. The results of the logistic regression yielded 8 statistically significant results for Genre: Adventure, Miscellaneous, Platform, Fighting, Racing, Shooter, Role-Playing, and Sports. Along with User Count, User Score, and Critic Count. The model explains a statistically significant and weak proportion of variance (P < 0.01) and can explain 27.5% of the variance in Global sales. Since there are many statistically significant variables. 

Lastly, I added the independent variable with control variables to my third model. I fitted a linear model to predict Global Sales with Critic Scores controlling for User Count, User Score, Critic Count, and Genre. The genre category that is missing is Action – one of them was used as a base category, as opposed to my base model. Strategy games were chosen less likely than action games however, platform games had more sales than action games. 
The results yielded 11 statistically significant results for Genre: Adventure, Miscellaneous, Platform, Puzzle, Racing, Shooter, Role-Playing, and Sports. User score, critic score, and critic count were also significant. The third model can explain 24.9% of the variance in Global sales. When I was controlling for both of them (IV +control), the coefficient for User Count got even higher. This is an indicator that it is an important variable. However, the strength of this relationship varies by genre. Strategy games, for example, have a relatively weak association, whereas puzzle games have a relatively strong association. Does the increase of critic rates cause customers to buy the game to play and leave a review? It seems like both variables have a moderating relationship with each other. User scores can be more important than we think.

Conclustion:
I think the relationship I’m not investigating in this study that may warrant more investigation is the relationship between User Count and Critic Score
People seem to HATE stratgey games 
