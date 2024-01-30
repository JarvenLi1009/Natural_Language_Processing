# Natural_Language_Processing

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Web_Scraping.ipynb
In this jupyternote, I used the Python requests library to initiate HTTP requests to obtain page content from the Trustpilot website and parsing the HTML source code using the BeautifulSoup library to extract data from the web pages.
Afterwards, I come up with a while loop to go over Trustpilot comment pages until at least 2,000 comments were collected. When the number of comments reached about a decent amount of data that I need, the while loop would stop.
Later on, I used for loops to extract key information precisely from each review page, including company name, the post date for that comment, the rating value the users put along with their comments, and then the review body itself.
The extracted data was organized in a structured format and exported to a CSV file to facilitate subsequent analysis and report.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Sentiment_Classification.ipynb
In this file, I build a text classifier model to conduct sentiment analysis, distinguish positive and negative comments by providing user reviews to the machine. The model will return whether the comment is positive or negative.
To break it into steps, I firstly manually categorized all of the reviews into positive and negative reviews based on the five ratings.
Then, I used Bag-of-Words to decompose the text documents into tokens, and standardized the text documents in each corpus by removing all the punctuations.
Afterwards, I used TF-IDF (term frequency) to turn text data into vectors for modeling.
In the model building steps, I trained a Multinomial Naive Bayes text classifier model using the vectorized text data.
Finally, I fine tuned text classifier model using grid search to improve the accuracy and precision of sentiment classification capability of my model.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Aspect_based_sentiment_analysis.ipynb
In this file, I developed an NER model to locate different dishes appeared in a customer's review and I built an ABSA model to determine whether a user's sentiment towards different dishes is positive or negative. 
Firstly, I utilized a customed NER model to accurately identify and locate different dishes names that appear in the reviews. 
Then I labeled all the dishes by adding specific tags to identify the beginning and end of each dish, providing clear data input to the sentiment analysis classifier.
Finally, I created an ABSA model to classify whether the user like or dislike a dish.
