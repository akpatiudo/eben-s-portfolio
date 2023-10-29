# Eben-s-portfolio
   ## HI THERE I'M EBENEZER AKPATI
[Data Speaks](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/cd730ca1-aba0-4ad2-bacb-a269a2ff0735)

## ABOUT ME
I am a Data Analyst and a Business Intelligence (BI) Analyst who love telling Stories with data. I have vitual project experience from top companies like Google, Pwc, KPMG, TATA, Accenture and Tritek Consulting.
I am proficient in communicating with data, when you speak the language of data, it talks back to you by revealing useful insights that can drive any sector positively.

## MY TOOLS
* R
* POWER BI
* TABLEAU
* EXCEL
* SQL SERVER
* Alteryx


## REACH ME @
[My linkedin profile](https://www.linkedin.com/in/ebenezer-akpati-9517aa23b/)
ebenezerakpati@gmail.com


## [Vist here for my pet projects](https://medium.com/@ebenezerakpati/data-analysis-project-with-sql-server-and-power-bi-2524bc650e39)

## [Project 1: Mrs Chatterjee Vs Norway: A Review Analysis of Twitter’s Perception Of The Movie.](https://github.com/akpatiudo/mrsChatter)
 
  **Use Case**
Viewing your Business from the prism of social media can change a whole lot about how you handle your business. An analysis like this can practically tell you what people feel about your goods and services. Sentiment analysis can give a company direction on what to do, thereby saving stockholders time and money. For Data Analysis Process
To make sense of any available data, a set of procedures must be completed. Identifying these procedures is essential as each stage is crucial in ensuring that the data is appropriately processed in a bid to offer useful and actionable information. Here are the steps I took in this process:

1	Data Gathering
2	Data Assessment and Cleaning
3	Data Processing
4	Data Analysis
5	Sentiment Analysis
6	Bigram Analysis and Network Definition
7	Data Visualization
8	Communications and Insights

## ![DashBoard](https://github.com/akpatiudo/ropo/assets/118566096/92718343-78be-4751-afa6-ad5f6491b1b0)

**Communication and Insights**
The top hashtag relating to the show was #MrsChatterjeeVsNowey. This would be as a result of the fact that it is the movie’s name, it makes sense for people to have made a tweet with the above hashtag and it’s only normal that people would want to continue with that for visibility case; a total 7.6k hashtags was made. This tweet is also the most liked and most retweeted this was followed by the major cast #RaniMukerji, it has 1.6k hashtag, this is natural consider how she spawned passion, anger, agony, love, persistence, emotions into her cast, tell the word the love and the pain of a mother whose kids have been taken away from her forcefully on the pretext of improper parenting.  
The sentiment analysis shows.  64.96% of Twitter had something positive to say about the movies, 23.74% were not happy with the movie, they have something negative to say and 11.3% where neutral about the movie

Based on the sentiment/emotional scores from tweets analysed I observe the following sentiments and their corresponding counts and percentages and I report from 10 and above: Anticipation: 8600 occurrences, accounting for approximately 13.2% of the sentiment score. Joy: 7146 occurrences, accounting for approximately 11.0% of the sentiment score. Negative: 6800 occurrences, accounting for approximately 10.0% of the sentiment score. Positive: 13746 occurrences, accounting for approximately 21.1% of the sentiment Trust: 11200 occurrences, accounting for approximately 17.3% of the sentiment score.

## [Project 2: Adidas Sales Project.](https://github.com/akpatiudo/Adidas-Sales-Project#adidas-sales-project)

## Part One 
## Residual Analysis: An R Project On How Adidas Quarterly Sales Are Affected By Quarter Of The year, Region, And By Product

## Introduction
This dataset is An Adidas sales dataset that have information on the sales of Adidas products, number of units sold, the total sales revenue, the location of the sales, the sales outlets and method of sales. This dataset is very granular, each row represents a line item for a purchase at one of 6 Retailers outlet spread across all the states in the five Region of USA. there is no missing value in this dataset. this project has three part to it, part one seeks to answer project statement using Residual analysis and part two seeks to use Dummy variables in regression to explain the project statement and part three, I want to give Adidas data insight on how not to over dependent on their best performing product using the decision tree algorithm to address this business problem.

## Residual Analysis Explaining the project statement

*  Best stores are Walmart and Sports Direct, best product is Women's Apparel 
   the store at Southeast beat their goal during second and third quarters for 2021 by at least $198,601.2
*  The store at South also beat its expectation during third and fort quarter by at least $154,993.3.
*  Worst stores are West Gear and Sports Direct in the West and South for Men's Athletic Footwear and Men's Street Footwear.
   The store at West missed its expected quarterly **oprating_profit** for first quarters of 2021 by at least $108,757.6.
*  The store in the South also missed its expected quarterly **oprating_profits** for third quarter in 2021 by about $102,934.7.
[Best Store](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/b10abbf2-b0ce-4a49-9326-64735ea39ab4)
[Quarter Performance](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/adeb418b-a9f3-49d2-bb61-362ddd7c4296)

## Recommendation 
The manager, may want to look into the two stores that under performed during 2021 to work on improving their performance. In contrast, He may want to look into the two stores that outperformed during 2021 to find out if their best practices can be replicated in other locations.

## Part Two 
## Residual Analysis: An R Project On How Adidas Quarterly Sales Are Affected By Quarter Of The year, Region, And By Product Part 2 " Using Dummy variables to analyse Adidas quarter of the year product performances

## Qualitative Variables
I Used Qualitative variable quarter of the year because machine learning algorithms, including regression, rely on numeric values. So we have to convert qualitative variables to numeric variables.

## Dummy Variables
What is often done is a series of binary variables is used to capture the different levels of the qualitative variable. Specifically, we would replace the quarter of the year variable, quarter_NoYear, with three variables: Second, Third, and Fourth. The values in these columns take on a value of 1 if the observation fits into that category, and a value of zero otherwise. We only need three columns because if they all have a value of 0, then that means the observation fits into the first quarter. Here's a dataframe to illustrate that idea with a bit more detail:

data.frame('quarter_char' = c('First', 'Second', 'Third', 'Fourth'), 'quarterSecond' = c(0, 1, 0, 0), 'quarterThird' = c(0, 0, 1, 0), 'quarterFourth' = c(0, 0, 0, 1))

## The Unique Effect of Quarter of the Year
Quarter of the year may have a significant effect on quarterly oprating_profit after controlling for the percentage of sales that come from other products. Let's test this out by including it with the unit_sold variables that we have already investigated
[Table](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/1f93d7e2-7a84-46fa-a2fd-421ff38417f8)

## Insight
regression analysis with the addition of the "units_sold" variable yields the following results:

The coefficient for the "units_sold" variable is 226.424 with a standard error of 1.152. This means that for each additional unit sold, the operating profit is estimated to increase by 226.424. The coefficient is highly significant (p-value < 0.001), indicating a strong positive relationship between units sold and operating profit.

The coefficient for the "quarter_charFourth" variable is 11,268.915 with a standard error of 696.438. This coefficient represents the difference in operating profit between the fourth quarter and the baseline quarter, while holding the number of units sold constant. The positive coefficient suggests that the fourth quarter tends to have higher operating profit compared to the baseline quarter.

All coefficients are highly significant (p-values < 0.001), indicating their strong relationship with operating profit.

The multiple R-squared value is 0.8019, indicating that the model with "units_sold" and quarterly variables explains approximately 80.19% of the variability in operating profit. The adjusted R-squared value is 0.8018, which takes into account the number of predictors in the model.

The F-statistic is 9756 with a p-value < 2.2e-16, indicating that the overall model is highly significant. This change is effectively communicated by visualizing the coefficients from all three models.
![image](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/75c27857-18c0-4940-badd-4bf0981cb297)

## Conclusion
Based on Model 2 and Model 3, it appears that the quarter_charThird variable had the largest positive coefficient and was statistically significant in both models. This suggests that the third quarter (quarter_charThird) had the most significant positive impact on the dependent variable compared to the other quarters (quarter_charFourth and quarter_charSecond). However, the practical significance and implications may vary depending on the specific situation or domain being studied.

## Part Three
## " Decision Trees: An Analysis To Predict Adidas Product With High Margin Profit"

## Introduction:
This analysis is squeal my work tittled Residual Analysis: How Adidas Quarterly Sales Are Affected By Quarter Of The year, Region, And By Product As an analyst, I want to give Adidas data insight on how not to over dependent on their best performing product. I will now use the decision tree algorithm to address this business problem. I assumed Adidas is planning for the future and would like to set up their business so they are not so reliant on selling their best product: Women's Apparel. One way to do that is to increase the sales of profitable products. Thus, Adidas would like to predict when a transaction is a going to be a sale of a high margin profit product. Profit margin is the percentage of gross profit to revenue, or revenue minus costs divided by revenue. It is a percentage of how much profit each product makes or what percentage of profit is earned for each dollar of revenue. I have to create the target veriable 'column' from 'Opreating_Margin'

## Insight

##Tree In Text Form
node), split, n, deviance, yval, (yprob) * denotes terminal node

root 7233 9425.0 high ( 0.6433 0.3567 )
Total_Sales < 22477 4305 4303.0 high ( 0.8005 0.1995 ) *
Total_Sales > 22477 2928 3968.0 low ( 0.4122 0.5878 )
6) Product: Men's Street Footwear,Women's Apparel 959 1291.0 high ( 0.5996 0.4004 )
12) Operating_Profit < 149813 733 1015.0 high ( 0.5184 0.4816 ) * 
13) Operating_Profit > 149813 226 180.7 high ( 0.8628 0.1372 ) * 
7) Product: Men's Apparel,Men's Athletic Footwear,Women's Athletic Footwear,Women's Street Footwear 1969 2471.0 low ( 0.3210 0.6790 ) *
In the given tree structure, the nodes are labeled numerically, and each node represents a decision point based on the specified condition. Here's the explanation of nodes 6 and 7 that houses Adidas Products:

# Node 6:
Split Condition: Product: Men's Street Footwear, Women's Apparel Number of observations (n): 959 Deviance: 1291.0 Predicted value (yval): high Probability of class high (yprob): 0.5996 (60%) Probability of class low (yprob): 0.4004 (40%) Decision: This node represents a subgroup of data where the product is either Men's Street Footwear or Women's Apparel. The majority class in this subgroup is high, with a probability of 0.5996. The deviance of 1291.0 indicates the level of impurity within this subgroup.

# Node 7:
Split Condition: Product: Men's Apparel, Men's Athletic Footwear, Women's Athletic Footwear, Women's Street Footwear Number of observations (n): 1969 Deviance: 2471.0 Predicted value (yval): low Probability of class high (yprob): 0.3210 (32%) Probability of class low (yprob): 0.6790 (67%) Decision: This node represents a subgroup of data where the product is either Men's Apparel, Men's Athletic Footwear, Women's Athletic Footwear, or Women's Street Footwear. The majority class in this subgroup is low, with a probability of 0.6790. The deviance of 2471.0 indicates the level of impurity within this subgroup. Comparatively, node 6 has a higher predicted probability for the high class (0.5996) compared to node 7 (0.3210). This suggests that the product category "Men's Street Footwear, Women's Apparel" (node 6) is more likely to have a high predicted value. However, it's important to note that these probabilities and predictions are specific to the trained classification tree and should be interpreted within the context of the dataset and the model's performance. No alt text provided for this image
![image](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/6859b0c7-61c3-448e-9c86-ee2755c2b5e4)

As we move through the tree, moving to the left is "No" while moving to the right is "Yes". "high" and "low" at the leaf nodes indicates that it is the prediction of the profitability of the purchase. We actually learn a lot that can help Adidas. The first, and most significant split that determines whether a purchase will be for a high or low margin profit is whether the purchases Men's Apparel,Men's Athletic Footwear,Women's Athletic Footwear,Women's Street Footwear or Men's Street Footwear,Women's Apparel. If the answer to this is yes, we move to the right of the tree and the product is very likely to be High profitability. For Men's Street Footwear, Women's Apparel, profitability is also predicted to be high, whether Opreating_profits is above or below $149,813.

## [Project 3: PWC DAVERSITY AND INCLUTION ANALYSIS SNIPPET](https://github.com/akpatiudo/diversity_inclusion/blob/main/README.md)
[Daversity And Inclusion](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/57bc7ca1-686b-47a5-a9c9-d60fd0cfd7a6)

[FY20 Promotion Analysis](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/d1bda34e-0816-4d93-a69b-3fec8516a60a)

[FY21 Promotion Analysis](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/6cac3349-97a0-4eec-bcd5-391873151cf8)

[Performance Rate Analysis](https://github.com/akpatiudo/eben-s-portfolio/assets/118566096/97a644d8-8a45-4f0d-801e-453d5e214822)









