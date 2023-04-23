# SC1015-DSAI-B128-Team-9

## About

Our project for SC1015 (Introduction to Data Science and Artificial Intelligence) analyses pokemon 

## Problem Definition

- Are we able to predict if a movie is good (rating above 7.2) based on its attributes?
- Which model would be the best to predict it?

## Models Used

1. Linear Regression
2. Random Forest Regression

## Conclusion

- Popularity and budget have low linear correlation value with ratings (watch out for bandwagons 🤣)
- Popularity of the casts and crews have higher linear correlation value with ratings
- Resampling imbalanced data improved model performance especially on the minority class
- Logistic Regression did not perform well with non-linearly correlated variables
- Neural Networks along with SMOTEENN resampling method consistently did well in predicting good movies after 100 training attempts (around 72% accuracy, 70% recall)
- Yes, it is possible to predict if a movie is good with acceptable amount of accuracy and recall

## What did we learn from this project?

- Collaborating using Google Colab
- How One Hot and Label Encoding work and when should they be applied
- Lambda functions to group different categorical values as one
- How Random Forest Regression and GridSearchCV work

## Contributors

- Long Ming Wei - Video Editing, Wrote code for Data Preparation and EDA, Fixed coding bugs in general
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
