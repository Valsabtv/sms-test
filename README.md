# SMS Spam Classifier📱
#### This is a machine learning project that classifies SMS messages into two categories: spam or ham (non-spam). It uses a Naive Bayes model along with TF-IDF for text vectorization to make predictions based on the content of the message.

## Features🌟
Text Classification: Classifies messages as either "spam" or "ham".

Model: Uses a Multinomial Naive Bayes model for prediction.

TF-IDF Vectorization: Converts text messages into numerical form to feed into the model.

Accuracy Evaluation: Evaluates the model using metrics like accuracy, precision, recall, and F1-score.

Confusion Matrix: Provides a confusion matrix for visualizing model performance.

## Prerequisites⚙️
Before running the project, make sure you have the following installed:

Python 3.x

Libraries: pandas, numpy, scikit-learn, seaborn, matplotlib

You can install the necessary libraries by running:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```
## How to Run
Prepare Your Dataset: Make sure your dataset (e.g., spam.csv) is ready. The dataset should have columns like "label" (spam/ham) and "message" (the text of the SMS).

### Run the Code:

Clone or download this repository.

Open a terminal or command prompt.

Navigate to the project directory.

### Run the script:
 ``` 
python spam_classifier.py
 ```
### View Results:

The classifier will output the accuracy of the model, the classification report, and the confusion matrix.

A file called report.csv will be saved with the detailed classification report.

## How It Works🛠️
### 1.Data Preprocessing:

The dataset is loaded, and the labels are encoded using LabelEncoder (ham = 0, spam = 1).

### 2.Vectorization:

The text messages are converted into numerical vectors using TF-IDF Vectorization, which captures the importance of each word in a message.

### 3.Model Training:

A Multinomial Naive Bayes classifier is trained on the training data to predict the labels (spam or ham).

### 4.Evaluation:

The model is tested on a test dataset, and its performance is evaluated using metrics like accuracy, precision, recall, and F1-score.

The confusion matrix is plotted to visualize how well the model is performing.

## Example📝 
Input:
```
predict_sms("Congratulations! You've won a free ticket to the Bahamas!")
```  
Output:
 ```
"spam"
```
