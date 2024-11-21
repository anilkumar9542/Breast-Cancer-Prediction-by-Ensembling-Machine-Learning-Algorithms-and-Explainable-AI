# Breast-Cancer-Prediction-by-Ensembling-Machine-Learning-Algorithms-and-Explainable-AI

Cancer, caused by abnormal cell growth, remains a leading cause of death worldwide. Among women, breast cancer significantly contributes to mortality rates, and its prevention is complex due to unknown causes. Advanced imaging techniques like mammography and ultrasound play a vital role in diagnosing breast cancer. 

This project employs **machine learning and Explainable AI** to predict breast cancer. By using data from fine needle aspiration (FNA) of breast masses, the model not only identifies whether a patient has breast cancer but also highlights which features of the cancerous cells are most influential. 

The machine learning algorithms used include **Random Forest**, **Gradient Boosting**, **AdaBoost**, and **Decision Tree**. The dataset was divided into 75% for training and 25% for testing. After training, the models were evaluated for their accuracy, as shown below:

| **Classifier**        | **Accuracy**   |
|------------------------|----------------|
| Random Forest          | 94.41%        |
| Gradient Boosting      | 92.31%        |
| AdaBoost               | 91.61%        |
| Decision Tree          | 81.82%        |
| **Proposed Model** (Random Forest + Gradient Boosting Ensemble) | **95.10%** |


The proposed ensemble model, combining Random Forest and Gradient Boosting, achieved the highest accuracy of 95.10%. This demonstrates its effectiveness in accurately predicting breast cancer while providing insights into the critical features influencing the diagnosis.

**SHAP (Shapley Additive Explanations)** interprets machine learning models by quantifying feature contributions using Shapley values. It enhances model interpretability and supports local/global analysis. In breast cancer prediction, SHAP identifies feature significance, where value changes indicate class shifts: increase/decrease suggests malignancy, while the opposite indicates benignity, aiding diagnosis transparency.

**WEB APPLICATION CREATION:**
The proposed model was saved as a pickle file and deployed using **Flask and Anaconda** is used for run time environment. The Flask application connects three HTML pages:  

1. **Home**: Provides brief information about breast cancer.  
2. **Input**: Allows users to input feature values.  
3. **Result**: Displays whether the prediction is benign or malignant, along with SHAP values for feature importance.

![Home](https://github.com/user-attachments/assets/1b8dac57-fa57-4325-84e1-9b46f1e64019)
![Input](https://github.com/user-attachments/assets/5553f361-123a-4ae6-ac81-4bef2fd6d9d4)
![Benign Prediction](https://github.com/user-attachments/assets/93adfea4-370a-429b-a47a-086cef7f2099)
![Malignant Prediction](https://github.com/user-attachments/assets/e0c0820c-2df7-4e17-9985-06817cc3d39a)

