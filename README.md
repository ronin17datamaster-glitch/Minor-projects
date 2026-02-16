# SPAM EMAIL CLASSIFICATION USING SUPPORT VECTOR MACHINE (SVM)

## 1. PROJECT OVERVIEW

This project implements a Spam Email Detection System using Machine
Learning. The model classifies SMS/email messages into:

-   Spam (1)
-   Ham / Non-Spam (0)

The classification is performed using a Support Vector Machine (SVM)
algorithm after applying text feature extraction techniques.

------------------------------------------------------------------------

## 2. OBJECTIVE

-   To analyze and visualize spam and non-spam messages.
-   To convert text data into numerical format.
-   To train an SVM classifier using different hyperparameters.
-   To evaluate model performance using accuracy, precision, recall, and
    confusion matrix.
-   To predict whether a new message is spam or not.

------------------------------------------------------------------------

## 3. DATASET INFORMATION

Dataset Name: SMS Spam Collection Dataset Source: UCI Machine Learning
Repository Total Messages: 5,572

Classes: - Ham (Non-Spam) - Spam

Dataset Structure:

## Label \| Message

ham \| Go until jurong point... spam \| Free entry in 2 a wkly comp...

------------------------------------------------------------------------

## 4. TECHNOLOGIES USED

-   Python
-   NumPy
-   Pandas
-   Matplotlib
-   Scikit-learn
-   Google Colab

------------------------------------------------------------------------

## 5. PROJECT WORKFLOW

Step 1: Data Loading - Dataset loaded using Pandas. - Labels converted:
spam -\> 1 ham -\> 0

Step 2: Data Visualization - Bar chart showing spam vs ham
distribution. - Pie chart showing percentage distribution. - Word
frequency analysis using Counter.

Step 3: Feature Extraction Used: CountVectorizer(stop_words='english')

-   Converts text messages into numerical feature vectors.
-   Removes common English stopwords.
-   Creates Bag-of-Words representation.

Step 4: Train-Test Split train_test_split(test_size=0.33,
random_state=42)

-   67% Training Data
-   33% Testing Data

Step 5: Model Training (SVM) Support Vector Machine classifier trained
with different C values:

C = 50 to 950 (step size 50)

Metrics recorded: - Training Accuracy - Testing Accuracy - Precision -
Recall

Best model selected based on: - Highest Precision - Highest Test
Accuracy

Step 6: Model Evaluation Evaluation metrics: - Accuracy - Precision -
Recall - Confusion Matrix

Confusion Matrix Structure:

                    Predicted Non-Spam    Predicted Spam

Actual Non-Spam True Negative False Positive Actual Spam False Negative
True Positive

Step 7: Prediction on New Message

Example: "You have won a lottery of \$2000. To claim it reply to this
email"

The model predicts whether the message is: - Spam or - Non-Spam

------------------------------------------------------------------------

## 6. PERFORMANCE METRICS

Accuracy -\> Overall correctness of the model Precision -\> Correct spam
predictions out of total predicted spam Recall -\> Correct spam
predictions out of total actual spam Confusion Matrix -\> Detailed
classification performance

------------------------------------------------------------------------

## 7. FUTURE IMPROVEMENTS

-   Use TF-IDF instead of CountVectorizer
-   Apply stemming and lemmatization
-   Compare with Naive Bayes and Random Forest
-   Deploy as a web application using Flask or Streamlit

------------------------------------------------------------------------

## AUTHOR

Your Name MSc Data Science Spam Email Classification Project
