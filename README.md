# Credit_Risk_Analysis

### **Purpose**
The following analysis main objective is to develop a Machine Learning Model to determine whether if an credit application has **High** or **Low** risk.

Given the nature of the challenge, several models were built and compared as shown on this document.

#

### **Results**
The initial approach consists of 6 different models which results are the following:

**ML. Models Summary**<br>
![Model_Summary](https://github.com/AxisAngeles/Credit_Risk_Analysis/blob/main/Challenge/Resources/Model_Summary.PNG)
<br> Based on accuracy, the main options are **Balanced Random Forest** and **Easy Ensamble AdaBoost** models.

* **Random Over Sampler:** 0.66 Accuracy | (High Risk) 0.01 Precision | (High Risk) 0.72 Recall
* **SMOTE:** 0.66 Accuracy | (HR) 0.01 Precision | (HR) 0.62 Recall
* **UnderSampling:** 0.54 Accuracy | (HR) 0.01 Precision | (HR) 0.69 Recall
* **SMOTEENN:** 0.64 Accuracy | (HR) 0.01 Precision | (HR) 0.67 Recall
* **Balanced Random Forest:** 0.77 Accuracy | (HR) 0.03 Precision | (HR) 0.64 Recall
* **Easy Ensamble AdaBoost:** 0.93 Accuracy | (HR) 0.09 Precision | (HR) 0.92 Recall

#

### **Conclussion**

As mentioned before, based solely on Accuracy Easy Ensamble should be an easy pick. However, given the main objective of the model, **precision** and **recall** indicators must be considered.

Overall, every model lacks in precision with poor results (less than 0.1). This means that eveery single model will deliver a lot of **False High Risk** assessments, which will result in lots of rejections.

When turning int **recall** indicator, Easy Ensamble rises also as the best option. This means, most of the **actual high risk applications will be detected**. Though, these results seem to good to be true and may benefit from a double check.

Based on above results, we conclude that a further analysis should be developed to improve precision on the models. This will include droping some of the less important variables and scaling some of the remaining variables.