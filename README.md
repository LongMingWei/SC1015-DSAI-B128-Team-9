# SC1015-DSAI-B128-Team-9

## About

Our project for SC1015 (Introduction to Data Science and Artificial Intelligence) analyses pokemon based on numerical and categorical variables to predict their weight using numerical regression methods

## Problem Definition

- Are we able to predict a pokemon's weight based on its other, even seemingly irrelevant attributes?
- Which model would be the best to predict it?

## Project/Code Outline

EDA
- Dropped variables that are definitely irrelevant to our problem statement (such as name)
- Removed a row with non-numerical data for capture rate and rows with null values of weight (make up a very small minority of our dataset)
- Analysed weight distribution and decided not to remove outliers as based on other distributions we analysed like height, outliers are still useful in predicting weight
- Analysed correlation of numerical variables with weight
- Converted certain numerical variables into categorical ones and analysed correlation of numerical predictors with weight (also analysed their count to see if their distributions/boxplots are reliable)
- Filled up missing values of percentage male and type2 to complete the above process
- Certain categorical variables like abilities and classification were ignored as there were too few datapoints for each unique category, resulting in their distributions not being reliable enough to predict weight 


Regression
- Grouped categorical values (with similar boxplots) of certain variables into one value and made new columns based on the new grouping using lambda function
- Used OneHotEncoder to split the categorical columns into separate new columns and put these new columns into a new dataframe
- Concatenating the new dataframe with the numerical variables, including the response, we get a clean and prepared dataframe for our Machine Learning segment 
- Fitted the new dataframe into linear regression and random forest regression models and analysed importance of variables

## Models Used

1. Linear Regression
2. Random Forest Regression

## Conclusion

- In most cases linear regression without outliers would work the best due to less overfitting/bias and our predictors (especially numerical ones) having strong linear relationship with weight, however the model's reliability will drop significantly for pokemon with weights being outliers
- We may need to gather more data of significant categorical variables outside our dataset to improve accuracy of model, as of now it’s very dependent on numerical continuous variables as categorical variables don’t show a strong enough correlation/pattern
- For now we will still use linear regression model without outliers to predict pokemon which seem to have average weight (as seen from their height or other factors), and linear regression with outliers for pokemon that are more likely to be outliers
- Random forest as of now is more prone to overfitting and takes longer to run as well due to having to process many decision trees and deciding factors, even more so with GridSearchCV

## What did we learn from this project?

- Collaborating using Google Colab
- How One Hot and Label Encoding work and when should they be applied
- Lambda functions to group different categorical values as one
- How Random Forest Regression and GridSearchCV work

## Contributors

- Long Ming Wei - Planned Project Outline and Content, Slide Design, Video Editing, Wrote code for Data Preparation and EDA
- Adam S Munaverali - Slide Design, Wrote code for EDA and Data Visualization
- Kevin Lai - Slide Design, Wrote code for Linear and Random Forest Regression

## References

Dataset
- <https://www.kaggle.com/datasets/rounakbanik/pokemon>

Learning sources beyond this course
- <https://www.geeksforgeeks.org/random-forest-regression-in-python/>
- <https://www.analyticsvidhya.com/blog/2020/03/one-hot-encoding-vs-label-encoding-using-scikit-learn/>

Images
- <https://www.mariowiki.com/Pokemon_Trainer>
- <https://www.pokemon.com/us>
- <https://www.nicepng.com/maxp/u2t4r5t4r5i1q8w7/>
- <https://www.deviantart.com/altiernate/art/Rosa-s-Thinking-Pose-Pokemon-Masters-808200485>
- <https://pokemon-fano.fandom.com/wiki/Poke_Ball>
- <https://www.pngaaa.com/detail/141338>
