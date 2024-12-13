# [Building a SVM Model for Classification - Wheat Seeds](https://nbviewer.org/github/tyrantdavis/svm-wheat-classification/blob/main/wheat-classification.ipynb)

## [Demo](https://nbviewer.org/github/tyrantdavis/svm-wheat-classification/blob/main/wheat-classification.ipynb)

A college department has shown interest in machine learning classification models. A professor from the Botany department aims to illustrate how the biological characteristics of seeds can influence their taxonomic classifications, such as their family, genus, and species. The professor has provided a dataset that includes various seeds and their physical traits. Unlike many datasets encountered in practical applications, the distribution of outcomes is balanced, with all three classes having the same frequency. 

This examination will allow classifying  samples consisting of kernels from three separate wheat varieties as Kama(1), Rosa(2), or Canadian(3).

This project will scope, analyze, prepare, plot data, and seek to explain the findings from the analysis.

### Scenario
During your discussions, it was discovered that the dataset may include outliers. Instead of opting for a logistic regression or decision tree model, a classifier utilizing Support Vector Machines (SVMs) will be developed. This approach is anticipated to enhance the model's effectiveness in classifying data that contains outliers.

The department aims to educate students about the various factors contributing to developing a seed's classification. Rather than simply delivering a traditional lecture and expecting students to absorb the information passively, the intention is to encourage them to draw conclusions and validate those insights through practical engagement. To achieve this, the plan is to develop a machine-learning model to facilitate this exploration. Utilizing a real-world dataset containing diverse statistics about seeds, the model will classify whether each seed belongs to one of three classes **Kama - Class 1**, **Rosa - Class 2**, or **Canadian - Class 3**. The goal is for students to input their data to see their hypothetical outcomes. This interactive approach enhances the lecture's relevance and provides an enjoyable academic experience. While the aim is to improve the user interface of the machine learning model in the future, the immediate focus is on establishing the foundational code.

**Features**

- Area
- Perimeter
- Compactness
- Length_of_kernel
- Width_of_kernel
- Asymmetry_coefficient
- Length_of_kernel_groove
- Class(123) - **target**

**Data Sources:**

- [UCI Wheat Seeds Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00236/seeds_dataset.txt)
  

## Project Goals
The objective is to classify seeds and educate students about the various factors that may contribute to their classification. 

Several questions will be asked:

- How does the Logistic regression boundary align with the data?
- How does the SVM regression boundary align with the data?
- What are the values for accuracy, precision, recall, and F1 scores?

#### Why use a support-vector machine algorithm to predict the classification?
Support Vector Machines (SVMs) are particularly effective for classification problems that involve training datasets containing outliers. In such scenarios, SVMs often demonstrate superior performance compared to logistic regression and various other classification methods.  A support-vector machine demonstrates significant efficacy in data classification, making it a suitable choice for the goals of this project. An instance of data can represent one category while simultaneously not belonging to another.


## Data
An anonymized dataset that can be used to train the machine-learning model has been found. It is a CSV file containing 210 observations with 7 predictor variables and 1 outcome(target) variable.  


## Conclusions
- How does the Logistic regression boundary align with the data?
    - The decision boundary struggles to effectively differentiate between the classes. A clear separation is present between the two categories, yet the space in between forms a line that the boundary fails to generalize adequately. This situation may suggest a possible problem of underfitting. Additionally, there has been a rise in the number of instances that were misclassified in the past.
- How does the SVM boundary align with the data?
    - The support vector machine (SVM) model demonstrates a significantly enhanced capability in generalizing the data and effectively distinguishing between the classes.
- What are the values for accuracy, precision, recall, and F1 scores?
    - The scores for the SVM model:
       - Accuracy: ~ 89%
       - Precision: ~ 89%
       - Recall: ~ 89%
       - F1: ~ 89%
