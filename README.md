Dataset
The project utilizes the Titanic dataset sourced from the Seaborn library.

Preprocessing & Data Cleaning

Feature Conversion: Qualitative variables such as sex, embarked, pclass, sibsp, parch, and survived were explicitly converted to categorical types to ensure proper treatment by machine learning algorithms.


Redundancy Removal: Redundant columns including alive, alone, deck, who, adult_male, embark_town, and class were dropped.


Missing Value Handling: * Missing values in the embarked column were imputed using the mode.

Missing values in the age column (approximately 20% of the data) were left as-is to avoid distorting the distribution and biasing survival analysis for specific age groups.

Exploratory Data Analysis (EDA) Insights

Survival Rate: The overall survival rate was approximately 38.38%, indicating a significant class imbalance.


Demographics: 75% of the passengers were under the age of 38, suggesting a young population trend.


Fare Distribution: Ticket fares showed a heavy right skew with extreme outliers, indicating a wide gap in passenger spending.

Model Development & Evaluation
Following the project requirements, three classification models were developed and compared:

Random Forest

Logistic Regression

Support Vector Machine (SVM)

Performance Comparison
Models were evaluated based on their accuracy on the test set:

Random Forest: 82.68%

Logistic Regression: 81.01%

SVM: 82.12%


Best Performing Model: The Random Forest model was identified as the top performer.

Detailed Assessment (Random Forest)
The Random Forest model correctly classified 148 out of 179 test samples. Its performance breakdown includes:


True Negatives: 92 (Strong identification of non-survivors) 


True Positives: 56 (Reasonable detection of survivors) 


Errors: 13 false positives and 18 false negatives 

Overall, the model demonstrates a reliable balance between precision and recall for this dataset.

Requirements Covered
[x] Choose at least three classification models.

[x] Identify the best-performing model.

[x] Describe insights from analysis steps.

[x] Interpret evaluation metrics for model performance.
