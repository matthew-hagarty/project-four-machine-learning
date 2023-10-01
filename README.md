# project-four-machine-learning

Objective:
  Using machine learning to predict election results and party vote percentages and swing states
  
Data Sources:
  Census Data: Collected data from the Census Bureau
  Election Results: 2000 to 2020 Election Results: dataverse.harvard.edu

Data Processing:
    Scale the data by using converting to percentage values
    Census Data: 
       Grouped into four categories: 
          -Gender 
          -Race 
          -Hispanic/Non-Hispanic descent
          -Age (under 50 percentage)
          -These categories were chosen to capture demographic factors that influence voting behavior
    Election Result: percentage voted Republican vs. Democrat 
Methods Explored:
    -Considered County/State data
      -Granularity
    -Focused on State level data 
    -Logistic Regression (Categorical):  Binary analysis. Winner: 1=Democrat, 0 = Republican
    -Linear Regression (Numerical):  predicting numerical vote percentages.
    -Multiple Linear Regression: multiple variables 
    -Polynomial Regression: Relationship between variables is nonlinear 
    -Assessed model performance using Mean Squared Error (MSE)
Method Evaluations:
  1. Logistic Regression model: Not suitable 
        -Dependent Variables/Features 
          -Census data 
          -Percentage voted for Democrat vs. Republic
          -Include as feature, model accuracy was 94%
          -Not included as feature, model accuracy was 74%
          -Consideration of including this feature 
          -Percentage vote is strong predictor of the election outcome 
          -Relevance to Goal of our analysis: goal is not to understand the relationship between voting patterns and       election results
          -Overfitting: including highly correlated features can lead to overfitting
  2. Linear Regression model:
     -Again, the linear model didn’t perform nearly as well, predicting Democrat victories every year
     -The Degree 3 and Degree 4 electoral vote predictions were most accurate
     -Based off of Winner
     -Both only mispredicted 2016, as did pollsters and political experts
     -Based off of difference in actual and predicted electoral votes won by each side
Future Improvements:
    -County Data
    -Working up from smaller data can give us more insight into each state’s specific demographics
    -More and Different Demographic Data
    -Socioeconomic Data
    -Population Density (Rural areas are typically more Republican, big cities more Democrat)
    -Education Level
    -Multiple categories for race, age, gender
    -Eligibility to Vote
    -Use of non-Demographic Data
    -People don’t vote along strict demographic lines
    -Options include: polling data, prior vote pattern by state

      

