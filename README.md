# Fake-News-Detection-Using-Voting-Classifier
For this particular project, I am using this dataset- https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets
You may easily download this dataset from kaggle.
![Screenshot (547)](https://github.com/user-attachments/assets/134779f0-5884-439a-b275-e16b0177dafa)


🛠️ Project Details: Fake News Detection
In this project, I worked extensively with TF-IDF vectorization for transforming the training, validation, and testing data.
Below is a detailed step-by-step explanation of the models used and the results achieved:
1. Vectorization Method-I utilized TF-IDF Vectorization (Term Frequency - Inverse Document Frequency) to convert the text data into numerical format.This approach captures the importance of words in the documents while reducing the influence of commonly occurring words.The TF-IDF vectorizer was applied consistently to the training, validation, and test datasets.

2. Machine Learning Models Trained-I trained several individual machine learning models on the TF-IDF-transformed data:

➔ Logistic Regression- simple yet powerful linear model. Achieved an accuracy of 98.2% on the validation data.

➔ Multinomial Naive Bayes-Particularly suitable for text classification tasks involving word frequencies. Achieved an accuracy of 93.2% on the validation data.

➔ Decision Tree Classifier-A tree-based model capable of learning non-linear decision boundaries. Achieved a very high accuracy of 99.54% on the validation data. A plot of the decision tree is provided below for visualization.

➔ Support Vector Machine (SVM)-Used with a linear kernel, as it is highly effective for text data. Achieved an accuracy of 99.34% on the validation data.

➔ Random Forest Classifier-An ensemble model consisting of multiple decision trees. Achieved an impressive accuracy of 99.54% on the validation data.

3. Ensemble Method: Voting Classifier-After evaluating the individual models, I implemented a Voting Classifier to further enhance the prediction performance:
The Voting Classifier was created by combining: (i). Random Forest Classifier (ii).Logistic Regression Model
This ensemble model aggregates predictions from both classifiers to make a final prediction, leveraging the strengths of each.

4. Performance of Voting Classifier-The Voting Classifier demonstrated strong performance: Accuracy on Validation Data: 99%
Accuracy on Test Data: 98.9%. This showed a slight improvement in generalization and robustness compared to individual models.

5. Visualization- To better understand how the Decision Tree model made its predictions, I visualized the structure of the trained Decision Tree.

The decision tree plot illustrates how the model splits data based on TF-IDF features to classify news as real or fake.
![Screenshot (548)](https://github.com/user-attachments/assets/a9734fb1-2b13-40f0-bf80-2b15c71f66d4)

✅ In summary, by applying TF-IDF vectorization combined with multiple powerful machine learning models — and finally ensembling the best ones — I was able to build a highly accurate fake news detection system achieving up to 99% validation accuracy and 98.9% test accuracy.
