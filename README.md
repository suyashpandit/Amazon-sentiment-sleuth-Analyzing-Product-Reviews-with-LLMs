# Amazon-sentiment-sleuth-Analyzing-Product-Reviews-with-LLMs
This model was developed as part of learning sentiment analysis using NLP techniques. Supervised learning methods for classification like LogisticRegression was used to build the model after preprocessing the dataset using NLTK. Using the TF-IDF vectorizer and learning the concepts behind it was a great learning experience. 

# Problem statement:
Customer reviews plays a huge role in whether a business flourishes or collapses. Online platforms like Amazon rely on these reviews to know the customer's opinion about the products as they do not have direct face to face interaction with the customers. These reviews are in text form, unstructured and varying in sentiment, often imbalanced with positive reviews being a lot more than negative reviews.

The amazon reviews dataset for amazon alexa is a highly imbalanced dataset with a majority of reviews being positive. However, we need to develop a sentiment analysis model using NLP techniques that can accurately classify customer reviews as positive or negative based on the text reviews provided. This helps for product improvement and increase customer satisfaction for buisinesses across online platforms.

# Evaluation Metrics:
Evaluation metrics are tools that allow us to measure how well a machine learning model performs its asks. They provide insights into a model's accuracy, relaibility and generalizing ability as well.

F1 score, precision and recall are better metrics than accuracy when using for classification task like this sentiment analysis. The imbalance in the distribution of the classes makes accuracy not a good metric although it is 90% in the above model. F-1 score is a better reflection of how the model handles both classes.

# Negative:

Precision: 0.43 --> High number of false negatives. When the model predicts Negative, it is wrong more than half of the time.
Recall: 0.80 --> Balancing the weight across the two classes helped improve recall. The model is identifying the negatives.
F-1 Score: 0.56 --> Harmonic mean of precision and recall. It is low as well because precision in this class is bad.

# Positive:

Precision: 0.98 --> When the model predicts positive, it is correct 98 percent of the time.
Recall: 0.91 --> Model correctly identified 91 percent of the actual positive reviews.
F-1 score: 0.94 --> Good F-1 score for this class.

# Conclusion:
This model was developed as part of learning sentiment analysis using NLP techniques. The dataset used was the Amazon customer review dataset of alexa from Kaggle. Supervised learning methods for classification like LogisticRegression was used to build the model after preprocessing the dataset using NLTK. The dataset was highly imbalanced with majority of the feedback being positive. Using the TF-IDF vectorizer and learning the concepts behind it was a great learning experience. Although I had already used LogisticRegression in the past, balancing weights between classes to improve the recall and seeing it change the results in realtime was really intriguing. The entire thought process has been documented in this documentation. Visualizing the result, creating the confusion matrix and going indepth into what it meant and how a confusion matrix shows the model performance result at a single glance was also eye-opening. In my future projects, I would like to learn more about balancing an imbalanced datasets using techniques like SMOTE or explore if there are other methods. This was a learning curve and I hope to apply a lot of this seamlessly in the projects ahead.
