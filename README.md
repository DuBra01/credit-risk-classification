# credit-risk-classification
📊 Credit Risk Classification Analysis 🚀

📌 Project Description

This project implements a Logistic Regression model to predict the status of a loan (healthy or high-risk). A dataset containing borrowers' financial information is used, and supervised learning techniques are applied to train and evaluate the model. 🔍📈

🛠️ Steps Taken

1️⃣ Data Loading and Preparation

✅ The file lending_data.csv was loaded into a Pandas DataFrame.
✅ Variables were separated into:

X (features): Borrower characteristics.

y (target): Loan status (0: healthy, 1: high-risk).
✅ The dataset was split into training and testing sets.

2️⃣ Training the Model with Original Data

🚀 A Logistic Regression model was instantiated and trained with the original data.
📊 Model performance was evaluated using:

Balanced Accuracy Score 🎯

Confusion Matrix 📉

Classification Report 📑
⚠️ A significant class imbalance was found (many healthy loans and few high-risk loans), which affected the model’s ability to correctly identify high-risk loans. ❌

3️⃣ Handling Imbalance with Oversampling

🔄 RandomOverSampler from imbalanced-learn was used to balance the classes by duplicating examples from the minority class (1).
🎯 The model was retrained with the balanced data.
📊 Performance was re-evaluated using the same metrics.

4️⃣ Results and Conclusions

✅ Balanced Accuracy Score improved to 0.9936 after oversampling. 🚀
✅ Recall for high-risk loans increased to 99% 📈, meaning the model is much better at detecting potential defaults.
⚠️ A slight increase in false positives (healthy loans classified as risky) was observed, which is an acceptable trade-off for minimizing loan defaults. 🔄

🏆 Final Conclusion

💡 Applying RandomOverSampler significantly improved the model's ability to detect high-risk loans, achieving a good balance between sensitivity and precision. 🔥
🎯 This highlights the importance of addressing class imbalance in classification problems to obtain fairer and more useful predictions. 💪📊
