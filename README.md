# Titanic Kaggle Competition Top 2%
This Jupyter notebook presents a comprehensive solution to the Kaggle competition, "Titanic - Machine Learning from Disaster" The primary objective of this competition is to predict whether a passenger survived the Titanic shipwreck based on attributes like passenger class, gender, age, etc. This is a binary classification problem. Through extensive data exploration, preprocessing, feature engineering, and model selection, my goal is to create a high-performing model capable of providing precise predictions for whether a passenger survived the Titanic. I have evaluated the model's performance using appropriate metrics and fine-tuned it to achieve the best possible results. Feel free to explore the notebook, understand the methodology, and experiment with different approaches to gain insights into the Titanic dataset and the machine learning process. If you have any questions or suggestions, please don't hesitate to reach out.

## Dataset Description
The dataset provides the ground truth label - whether each passenger survived or not, represented as 0 for no and 1 for yes. Each observation also contains attributes providing insights into the social status and privileges of each person on board:
 - Pclass: The passenger's cabin class on the ship (1st, 2nd or 3rd class)
 - Name: The name of the passenger
 - Sex: Male or female
 - Age: The age of the passenger
 - SibSp: The number of siblings and spouses with the passenger
 - Parch: The number of parents and children with the passenger
 - Ticket: The ticket number
 - Fare: How much the passenger paid for the ticket
 - Cabin: Which cabin the passenger was allocated
 - Embarked: Which port the passenger boarded from

## Approach
My approach to tackling the Titanic Kaggle competition involved a systematic and well-structured methodology, which can be summarized into the following key steps:
 1. Exploratory Data Analysis (EDA):
    I started by performing Exploratory Data Analysis on the provided dataset. EDA allowed me to gain a deeper understanding of the data, its distribution, and uncover any potential patterns or insights. By visualizing and summarizing the data, I could identify the relationships between different features and the    
    target variable - whether a passenger survived or not.

 2. Data Preprocessing:
    Data preprocessing is crucial to ensure the data is suitable for training machine learning models. In this step, I addressed missing values, which can significantly impact model performance. Additionally, I leveraged the "Name" feature to extract the titles (e.g., Mr., Mrs., Miss) and converted them into a more 
    concise representation containing only the first letter of each title. This simplified the data and potentially provided a new feature that could contribute to predicting survival.

 3. Adding Additional Data:
    To enhance the predictive power of the model, I explored the possibility of incorporating additional relevant data. This could could be derived from the existing features. By intelligently augmenting the dataset, I aimed to provide the model with more information to make 
    accurate predictions.

 4. Handling Missing Values:
    Missing values can introduce bias and hinder model performance. Therefore, I employed various techniques, such as imputation, to fill in missing values for relevant features. By carefully addressing missing data, I aimed to ensure the model's robustness and generalizability.

 5. Hyperparameter Tuning:
    Machine learning models often come with hyperparameters, which are parameters that cannot be learned during training and need to be set beforehand. To optimize the model's performance, I performed hyperparameter tuning using techniques optuna. By systematically searching through different combinations of 
    hyperparameters, I aimed to find the best configuration for each machine learning algorithm, leading to improved predictive performance.

 6. Modeling and Ensemble Methods:
    For the core of the predictive task, I experimented with several machine learning algorithms, such as Random Forest, XGBClassifier, LGBMClassifier, LogisticRegression, and others. Each algorithm has its strengths and weaknesses, and by trying multiple approaches, I could    
    identify the best-performing model for this specific problem.
    To further boost the model's performance, I employed ensemble methods, I employed the VotingClassifier, a powerful technique that combines multiple individual machine learning models to make collective predictions. The idea behind the VotingClassifier is to take advantage of the diverse strengths and capabilities 
    of various models and create a more robust and accurate prediction ensemble.

## Result
In the Titanic Kaggle competition, the primary evaluation metric used to assess the performance of our predictive model was accuracy. Accuracy is a widely-used metric for binary classification problems, measuring the percentage of correct predictions made by the model among all the predictions.
After extensive data exploration, preprocessing, feature engineering, and modeling, my predictive model achieved an impressive accuracy score of 0.81100 on the test dataset. This means that approximately 81.1% of the passengers' survival status was correctly predicted by my model.
I am thrilled to announce that my submission achieved a remarkable rank of 295 out of 16,204 participants. This outstanding result places my model among the top 2% of all submissions, highlighting its effectiveness and the strength of my approach.
![Screenshot 2023-07-28 230347](https://github.com/fawazatha/Titanic-Kaggle-Competition/assets/132468764/d5c812ed-acaa-4018-8254-be4f376afbc6)
![Screenshot 2023-07-28 221556](https://github.com/fawazatha/Titanic-Kaggle-Competition/assets/132468764/127b850a-cea2-4535-b1f1-a035c6f1b4e7)
