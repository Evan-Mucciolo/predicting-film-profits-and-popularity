# predicting-film-profits-and-popularity

## Introduction

We set out to take a dataset of movies from all across the world to attempt to answer the question, can we predict which movies are profitable?

## Defining Profitability
What makes a movie 'profitable'? We had to find a couple of ways to answer this question and we had three attempts. The simple revenue less the film's budget was our first thought. This worked well, although it did not capture the return on investment for what someone put into a movie. To capture that, we created a profit percentage in hopes that this would create an even playing field between high and low budget movies. Lastly, we tried comparing to an industry standard found online, a 10-20% profit margin. This proved difficult as we did not have enough data available to find our profit margins, as that includes more than a simple calculation of revenue less the budget.

## Data Cleaning

The dataset we began with had around 1 million records, which we thought would be more than enough to find trends and come up with some kind of prediction that was reliable. During the data cleaning process however, that number dwindled to around 10,000 records. The dataset we had chosen turned out to be incomplete in a lot of columns, starting with release date, and even when it came to budget and revenue. This made our cleaning a bit difficult but ultimately we ended with a dataset that included: month of release, season of release, adult vs non adult film (rated R or not), budget, genre, and keywords in the movie description such as 'Superhero'. 

## Model Selection

We chose to take a stab at using supervised learning models that could be used to predict a binary outcome: Logistic Regression, Decision Tree, and Neural Network. Each model more complex than the last, we thought the added complexity would be necessary as it seemed to us that it would be difficult to predict a movie's profitability based on the features we had available in our dataset. 

## Model Results

Logistic Regression: 65% Accuracy, 98% Recall, 65% Precision
Decision Tree: 58% Accuracy, 65% Recall, 65% Precision
Neural Network: 62% Accuracy, 80% Recall, 67% Precision

## Model Recommendation
Based on our low accuracy and low precision across the board, we would not recommend any of the models for use. It is not good at predicting outcome in any scenario, a 65% accuracy could result in many investments with poor results. Lastly, it does not answer the most important questions, how much money will the film make? If you lose $20 on 100 films, but make $100,000,000 on one, you will have a profit overall. This model needs to take into account profit size to be used for any sort of recommendation moving forward. 

## Future Changes
In order to create a better model, we would change our defintion of what is considered profitable. To do this, we likely would have to bucket the films into high and low budget, as well as high/low grossing to get a better idea of the outcome our predictions could result in. 

## Additional Resources
The data source for this project is too large to be uploaded to GitHub. It can be found here on Kaggle: https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies?resource=download

Our Google Slides presentation can be found here: https://docs.google.com/presentation/d/1aRi58ID9QZL5j37T6c6XrENEktiXhBPBefzpAJuFx00/edit?usp=drive_link
