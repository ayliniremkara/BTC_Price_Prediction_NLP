# btc-price-prediction-sentiment-analysis

Predicting Bitcoin price fluctuations is becoming
important for organization and investors. Some methods can generate investment ideas
by predicting the movement of Bitcoin prices in the future. One of the methods that can help
in predicting Bitcoin prices is sentiment analysis. 

In this project, two different GUIs were created one of these GUIs contained the first
prediction system and the other contained the second prediction system. In the first model,
the user is expected to enter only the news title. Based on this news headline and obtaining
the BTC price of the relevant day, it calculates the sentiment score and estimates the BTC
price change for tomorrow compared to today. In the second model, the user is expected
to enter the news title, USDI, and Dow Jones financial values. It calculates the sentiment
score based on the news headline received from the user and predicts how the BTC price will
change tomorrow depending on the financial metrics it receives, today’s BTC price, and the
calculated sentiment score.

From May 10, 2023, to May 11, 2020, Bitcoin news was collected. VADER,
GPT-3, TextBlob, and CryptoBERT were used to give sentiment scores to this dataset. Since
it was seen that the most accurate scores were given by VADER, the project continued with
the data scored with VADER. The BERT model was trained with this dataset scored by the
VADER. After receiving a text from the user for both models, the sentiment score is calculated
with the BERT model. For two different prediction systems, models were constructed and
trained using SVM, Random Forest, and Logistic Regression algorithms. Each prediction
algorithm was trained with both the original training data and the training data prepared using
SMOTE-Tomek.

The performances of the models created for two different prediction systems were exam-
ined. When comparing the performances, two different scenarios that are buying and selling

BTC were considered. For the first prediction system, considering the first scenario, the

model created with SVM and trained with resampled data gives the best results, and consid-
ering the second scenario, Random Forest models give the best results. One of these Random

Forest models is trained with original training data and one with balanced data. When the
models selected successfully for the first scenario, the confusion matrices are examined. It
is seen that the cases where the prediction value is ’+1’ and the actual value is ’-1’ are less
than the other models. In this case, users, who want to buy BTC, can be provided with a less
risky recommendation. For this reason, it is more appropriate to use the model created with
SVM and trained with resampled data for the first scenario in the first prediction model. 
In the second scenario, successful algorithms were selected by looking at the confusion matrix.
Models with the lowest outputs where the prediction value is ’-1’ and the actual value is ’+1’
were found to be more appropriate for this scenario. Thus, it was ensured that users who
want to sell BTC can get a more reliable recommendation.

In the second prediction system, for the first scenario, models created using Logistic
Regression and using SVM give the best results. Both models are trained with resampled

training data. These SVM and Logistic Regression models give more reliable recommenda-
tion when looking at confusion matrices than other prediction models. In the first scenario, it

is desirable to have a minimum of situations where the prediction will rise but the true value
will fall. Models prepared with SVM and Logistic Regression and trained with resampled
data have this undesirable situation less than others. For the second prediction system, the
Random Forest model trained with the original training set gives the best performance in the
second scenario condition. In this second scenario, it is desirable to minimize the fact that
the price of BTC is predicted to decrease while actually rising, as more reliable advice is

provided to users who want to sell. Compared to other models, looking at the confusion ma-
trices, the Random Forest model contains less this situation output for the second prediction

system and the second scenario. Other models contain more cases with prediction value ’-1’
while more actual values are ’+1’ in confusion matrices.

In addition, the classification successes of the developed prediction models for each class
were compared. For the first prediction system, Random Forest models and the SVM model

trained with balanced data were able to classify into all three classes. However, Logistic Re-
gression models and the SVM model trained with original data could only classify in a single

class. In general, each prediction model made the best classification in the ’0’ class. When
the models created for the second prediction system are examined, the Logistic Regression
model trained with balanced data, Random Forest models and the SVM model trained with
balanced data can be classified in every class. Logistic Regression trained with the original
data and SVM models trained with the original data could only classify in the ’0’ class.



