# Machine Learning to Predict Credit Card Fraud


# Objective:
To build a an optimised machine learning model that predicts credit card fraud using data sourced from anonymous transactions.
This model build will help financial institutaions to detect and prevent fradulant transactions.


# Dataset:
The dataset encapsulates credit card transactions sourced from European cardholders throughout 2023. 
Constituting a formidable dataset of over 550,000 records, the data undergoes rigorous anonymisation protocols to safeguard the identities and locations of the cardholders. 
Our primary directive revolves around harnessing this dataset's potential to refine and enhance our data model, enabling the discernment of fraudulent activities within the financial landscape with greater precision and efficiency.

Dataset source: https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023?resource=download

Features of the dataset (columns):
    id:     Unique identifier for each transaction
    V1-V28: Anonymised features representing various transaction attributes (e.g., time, location, etc.)
    Amount: The transaction amount
    Class:  Binary label indicating whether the transaction is fraudulent (1) or not (0)

Link for initial data download: https://drive.google.com/file/d/1erGe3UGlc7TjqQ8iwNN_elZ9VP2bTmXz/view?usp=sharing


# Importing the Data
Data importation was conducted systematically by constructing a connection string and creating a SQLAlchemy engine. This ensured a robust and efficient process for accessing the dataset.


# Data Cleaning
Utilising Python Notebook, the data cleaning procedure was executed. Non-float values were accurately converted to NaN, and subsequently, all rows containing NaN values were systematically removed. This cleaning process ensured the elimination of any anomalies present in the dataset, thereby enhancing its integrity and reliability.


# Model Implementation and Optimisation

# Model 1 - Logistic Regression
Following the comprehensive data cleaning phase, our focus shifted towards the development and optimisation of a supervised learning model. For our initial model build, we chose Logistic Regression due to its aptitude for binary classification tasks, a characteristic fitting for transactions typically classified as either fraudulent or legitimate. Moreover, Logistic Regression's ability to scale efficiently to large datasets made it an appealing choice for our analysis.

This iterative process involved fine-tuning of model parameters and evaluation of performance metrics to achieve optimal predictive capabilities. To our surprise, the accuracy of this model surpassed our expectations, achieving an impressive accuracy rate of 99.84%. Subsequent attempts at further optimisation yielded identical results, solidifying the robustness of our approach.

While Logistic Regression proved to be a commendable choice, it is not without its limitations. Acknowledging the necessity for exploring alternative methodologies, we proceeded to explore the efficacy of decision trees in our modeling endeavors.


# Model 2 - Decision Tree
After achieving remarkable success with Logistic Regression, our team opted to explore alternative modeling approaches to further enhance predictive performance. Decision trees emerged as a compelling candidate for our next model build due to several reasons. Firstly, decision trees offer interpretability, enabling us to easily understand and visualise the underlying decision-making process. Additionally, decision trees are capable of capturing nonlinear relationships and interactions between features, which can lead to improved performance, especially in complex datasets such as credit card transactions. After experimentation and parameter tuning, our decision tree model surpassed our expectations, achieving an outstanding accuracy rate of 99.95%. This exceptional performance underscored the effectiveness of decision trees as a robust modeling technique for credit card fraud detection.

With the accuracy and predictability climbing close to 100% we decided to try another model build using Random Forest.


# Model 3 - Random Forest
For our final model build we opted for Random Forest as our preferred method for credit card fraud detection due to its exceptional accuracy and several advantageous characteristics. Random Forest's ability to combine multiple decision trees, handle complex data relationships, identify important features, scale to large datasets, and handle imbalanced data made it a natural choice for our task. Analysts also favored Random Forest for its proven track record of accuracy and reliability in fraud detection tasks. After thorough experimentation and parameter tuning, our Random Forest model surpassed expectations, achieving an outstanding accuracy rate of 99.97%. This exceptional performance underscores the effectiveness of Random Forest as the most reliable method for detecting fraudulent credit card transactions with unparalleled precision and reliability.


# Conclusion
In conclusion, our journey to predict credit card fraud through machine learning has yielded remarkable results. Beginning with data sourced from anonymised transactions, we embarked on a mission to refine our model to enhance fraud detection capabilities. Through meticulous data cleaning and strategic model implementation, we surpassed expectations at every turn. From Logistic Regression to Decision Trees and ultimately to Random Forest, each model iteration outperformed the last, culminating in a Random Forest model with an outstanding accuracy rate of 99.97%. This exceptional performance solidifies Random Forest as the optimal method for detecting fraudulent credit card transactions, providing banks and financial institutions with a robust tool to safeguard against fraudulent activity. Our endeavor underscores the power of machine learning in combating financial crime and underscores the importance of ongoing innovation and refinement in fraud detection methodologies.


Thank you!
