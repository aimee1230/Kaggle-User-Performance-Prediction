Kaggle User Performance Prediction 🚀

Overview

This project analyzes Kaggle user engagement, competition participation, and performance using machine learning. By leveraging classification and regression models, we predict key metrics such as gold medal achievements, competition performance tiers, and dropout risks.

Objective

Predict gold medal achievements based on user competition history and engagement.
Classify users into competition performance tiers using past performance and activity levels.
Identify inactive users (dropout risk) based on engagement patterns.
Predict a user's overall performance tier based on participation across competitions, notebooks, datasets, and discussions.
Dataset

The dataset consists of Kaggle users and includes the following key features:

Key Features:
User Engagement: Competition participation, submissions, notebooks, datasets, discussions.
Performance Metrics: Medals (gold, silver, bronze), performance tiers (competitions, notebooks, datasets, discussions).
Activity Trends: Registration date, elapsed days since registration, last content shared.
Recognition Factors: Followers, upvotes received on notebooks and datasets.
Technologies Used

Programming Language: Python 🐍
Libraries: Scikit-Learn, XGBoost, Random Forest, MLP, SVC, Decision Tree, Pandas, Matplotlib, Seaborn
Approach & Methodology

1️⃣ Data Preprocessing & Feature Engineering
Handled missing values and outliers.
Converted categorical data using Label Encoding.
Normalized numerical features using StandardScaler for models sensitive to scale (MLP, SVC).
2️⃣ Exploratory Data Analysis (EDA)
Visualized user activity trends (competitions, notebooks, discussions).
Analyzed correlation between performance tiers and engagement metrics.
Examined feature importance to determine key factors influencing user success.
3️⃣ Machine Learning Models & Predictions
1. Predicting Gold Medal Achievements 🏅

📌 Target: GoldCompetitionMedals
🔹 Features:

Competition count, submission count, performance tiers
Followers, dataset and notebook upvotes
🔹 Models Used:
✅ Random Forest Regressor
✅ MLP Regressor

2. Predicting Competition Performance Tier 🎯

📌 Target: CompetitionsPerformanceTier
🔹 Features:

Competition participation, submissions, medals won
Performance across competitions, notebooks, datasets, discussions
🔹 Model Used:
✅ Support Vector Classifier (SVC)

3. Predicting User Dropout Risk (Inactive Users) 📉

📌 Target: LastContentDaysElapsed (Higher value = Higher dropout risk)
🔹 Features:

Elapsed days since registration
Competition, notebook, dataset activity
Performance tiers
🔹 Model Used:
✅ XGBoost Regressor

4. Predicting Overall User Performance Tier 🏆

📌 Target: PerformanceTier
🔹 Features:

Competition, dataset, notebook, discussion performance tiers
Competitions participated in, notebooks created
🔹 Model Used:
✅ Decision Tree Classifier

4️⃣ Model Optimization & Evaluation
Each model was optimized using hyperparameter tuning and evaluated with relevant metrics:
✅ Regression Models: Evaluated using MAE, RMSE, R² Score
✅ Classification Models: Evaluated using Accuracy, Precision, Recall, F1-Score

Results & Insights

📌 Gold Medal Prediction: More competitions and high submission counts significantly impact medal achievements.
📌 Performance Tier Classification: Medal count and submission frequency are strong indicators of competition success.
📌 User Dropout Prediction: Less engagement in notebooks/datasets and long inactivity periods increase dropout risk.
📌 Feature Importance Analysis: Competition history, performance tiers, and engagement levels are key predictors.
