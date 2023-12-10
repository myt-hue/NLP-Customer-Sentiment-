# NLP-Customer-Sentiment for Google and Apple Products
![image](https://cdn.cultofmac.com/wp-content/uploads/2012/07/AppleTwitter1.jpg)

Authors: Mytreyi Abburu, Marley Lopez, Dan Rosen

## Business Overview
Build a model to predict negative emotion displayed in tweets diplayed in Apple products

## Data Understanding
The dataset is from CrowdFlower containing 9092 tweets. The limitations for the dataset are imbalanced data and demographic bias. We filtered our dataset by company, Apple, and whether the tweets were negative or positive. The final dataset contains 2337 tweets. 

## Data Analysis
In order to determine which tweets are directed towards Apple, we created a numerical column to identify whether the brand is Apple or not. In a new numerical column, we categorize the type of emotion in the tweet as positive, negative, or neutral. Neutral includes instances where there was no emotion toward a brand or product found or where the evaluator couldn't tell.  Furthur, we constrained our dataset to only include postive and negative tweets for Apple Products and removed columns that we do not need. Next, we utilized a function to handle the preprocessing steps of NLP(Removing stopwaords, removing capitalization, lemmitization).The model providing our best result for its accuracy in predicting the correct type of emotion was the base Multinomial Naive Bayes model with count vectorization. This model gave us the highest precision score as well, so it is the best at avoiding the identification of a negative tweet as one with positive sentiment.
Main Finding

### Frequency Distribution of Top 5 Words
![image](https://github.com/myt-hue/NLP-Customer-Sentiment-/assets/73657823/ee4a231e-8a6d-415e-b67b-26d533ef439d)

The most commonly tweeted word was 'IPad'.

### Number of Product Mentions in Tweets
![image](https://github.com/myt-hue/NLP-Customer-Sentiment-/assets/73657823/652b2e2f-5905-4cf9-ac10-7b054d9bbf5d)

IPhone has a larger ratio of Positive to Negative Tweets

### Common Words in Negative Tweets
![image](https://github.com/myt-hue/NLP-Customer-Sentiment-/assets/73657823/4a5bb3b0-13b2-4dc8-8bdb-ed0daf0b47e2)

## Conclusions
Our model predicts negative tweets with 88% accuracy. Concerns surrounding the iPhone are battery life and SXSW iPad rollout.

## Future Insights 
Balance Tweet Samples 
Study RT's effect on sentiment
Accurate Tagging

## Repository Structure 
├── Data                             <- Data file used in this project
├── Image                            <- Images and Graphs used in this project obtained from external and internal source
├── .gitignore                       <- Contains list of files to be ignored from GitHub
├── presentation.pdf   <- Slide Presentation of the project
├── README.md                        <- Contains README file to be reviewed    
└── index.ipynb                      <- Jupyter notebook of the project containing codes and analysis

