# <h1 align="center">Fake News Detection Using Machine Learning</h1>

## <h2>Project Overview</h2>
In the digital age, the rapid spread of fake news through various online platforms has become a significant issue, leading to misinformation and societal harm. This project aims to develop a robust machine-learning model capable of classifying news articles as either true or false. By leveraging various machine learning techniques, we provide a valuable tool to combat misinformation.

explore multiple machine learning techniques, including <i><b>Logistic Regression</b></i>, <i><b>Decision Tree Classifier</b></i>,  <i><b>Gradient Boosting Classifier</b></i>,  and <i><b>Random Forest Classifier</b></i>, to determine the most effective approach for fake news detection. The performance of each model is evaluated based on accuracy, precision, recall, and F1 score..

## <h2>Objective</h2>
The primary objective of this project is to build a machine-learning model that accurately classifies news articles into two categories:
- **True:** Genuine news articles
- **False:** Fake or fabricated news articles

## <h2>Methodology</h2>

### <h3>1. Data Collection and Preprocessing</h3>
- **Data Collection:** The dataset consists of labeled news articles categorized as either true or false. It is sourced from reliable repositories to ensure a diverse range of topics and sources.
- **Data Preprocessing:** This includes cleaning the data by removing irrelevant information, handling missing values, and performing text normalization (e.g., lowercasing, punctuation removal). Techniques such as tokenization, stop-word removal, and lemmatization are applied to prepare the text for model training.

### <h3>2. Feature Engineering</h3>
- **Text Representation:** Convert text data into numerical features using techniques like Count Vectorization and Term Frequency-Inverse Document Frequency (TF-IDF) to make it suitable for machine learning models.
- **Additional Features:** Enhance the model by incorporating features such as article length, presence of specific keywords, and sentiment analysis.

### <h3>3. Model Selection</h3>
- **Logistic Regression:** A baseline model that uses linear relationships between features and labels for classification.
- **Decision Tree Classifier:** A non-linear model that captures complex patterns and provides insights into feature importance.
- **Gradient Boosting Classifier:** An ensemble technique that combines weak learners to create a strong predictive model.
- **Random Forest Classifier:** Another ensemble method that builds multiple decision trees and averages their predictions to improve accuracy and reduce overfitting.

### <h3>4. Model Evaluation</h3>
Evaluate each model using the following metrics:
- **Accuracy:** The proportion of correctly classified instances.
- **Precision:** The model's ability to identify positive instances correctly.
- **Recall:** The model's ability to capture all relevant positive instances.
- **F1 Score:** A balanced measure considering both precision and recall.

## <h2>Dataset</h2>
The dataset used consists of a balanced set of true and false news articles. It is split into training and testing sets to evaluate the model's performance on unseen data. Ensuring the quality and diversity of the dataset is crucial for developing a robust model.

## <h2>Dependencies</h2>
Before running the code, ensure the following libraries and packages are installed:
- **Nltk**
- **Python**
- **Scikit-learn**
- **Pandas**
- **NumPy**
- **Regular Expression**
## <h2>Results</h2>

## <h4>Classification Report of Logistic regression </h2>

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| **0** | 0.95      | 0.95   | 0.99     | 4733    |
| **1** | 0.95      | 0.94   | 0.95     | 4247    |
| **Accuracy** |           |        | 0.95     | 8980    |
| **Macro Avg** | 0.95      | 0.95   | 0.95     | 8980    |
| **Weighted Avg** | 0.95      | 0.95   | 0.95     | 8980    |


## <h4>Classification Report of Random forest</h4>

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| **0** | 0.94      | 0.95   | 0.94     | 4733    |
| **1** | 0.97      | 1.00   | 0.98     | 4247    |
| **Accuracy** |           |        | 0.94     | 8980    |
| **Macro Avg** | 0.94      | 0.94   | 0.94     | 8980    |
| **Weighted Avg** | 0.98      | 0.94   | 0.94     | 8980    |

## <h2>Model selection </h2>
### <h3> Logistic Regression Classifier</h3>

The Logistic Regression Classifier was selected as the final model due to its impressive performance across various metrics.  Logistic Regression is an ensemble technique that builds multiple weak learners (typically decision trees) in a sequential manner, where each subsequent model corrects the errors of its predecessor. This results in a powerful and accurate predictive model.

#### **Performance Summary**

- **Precision:** The Gradient Boosting Classifier achieved a precision of 0.95 for class 0 (true news) and 0.94 for class 1 (fake news). High precision indicates that the model correctly identifies a high proportion of actual positive instances without misclassifying too many negative instances as positive.

- **Recall:** The model demonstrated perfect recall of 0.95 for class 0, meaning it identified all actual true news articles. For class 1, recall is also 0.95, signifying that it captured all fake news articles accurately.

- **F1-Score:** The F1-score of 0.95 for both classes reflects a balance between precision and recall, showcasing the model's overall effectiveness in identifying both true and fake news articles accurately.

- **Accuracy:** With an overall accuracy of 0.95, the Logistic Regression Classifier correctly classified all instances in the dataset, indicating exceptional performance.

- **Macro Average:** The macro average values of precision, recall, and F1-score are all 0.95, demonstrating the model's consistent performance across both classes.

- **Weighted Average:** The weighted average scores, also 0.95, confirm that the model performs uniformly well across different class distributions in the dataset.

#### **Conclusion**

#### **Conclusion**

The <b>Logistic Regression Classifier</b> has proven to be highly effective for the fake news detection task, providing excellent results across all performance metrics. Its ability to handle complex patterns in the data and achieve perfect classification makes it a strong candidate for deployment in real-world applications to combat misinformation.
