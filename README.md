# California Housing Prediction

This project aims to predict housing prices in California using a machine learning approach. By analyzing a dataset containing various features related to housing, such as location, size, and proximity to the ocean, we can develop a model that accurately predicts housing prices.

## Dataset
The dataset used in this project consists of information on housing in different regions of California with following features:

* longitude: A numerical value representing the longitude of the district.
* latitude: A numerical value representing the latitude of the district.
* housing_median_age: The median age of the houses in the district.
* total_rooms: The total number of rooms in the district.
* total_bedrooms: The total number of bedrooms in the district.
* population: The total population of the district.
* households: The total number of households in the district.
* median_income: The median income of households in the district.
* median_house_value: The median value of houses in the district (the target variable).

## Methodology
To predict housing prices, we followed the following steps:

1. Data Preprocessing: We started by exploring and cleaning the dataset. This involved handling missing values, removing duplicates, and addressing any outliers or inconsistencies in the data.

2. Feature Encoding: As part of the preprocessing step, we encoded the categorical feature "ocean_proximity" using label encoding.

3. Train-Test Split: We split the dataset into a training set (80% of the data) and a test set (20% of the data). The training set was used to train the machine learning models, while the test set was used to evaluate their performance.

4. Feature Scaling: To ensure that all features have a similar scale, we applied the StandardScaler to the numerical features. This transformation helps in preventing certain features from dominating the learning process due to their larger magnitude.

5. Model Selection: For this project, we used two machine learning algorithms: Decision Tree and Random Forest. Decision Tree is a simple and interpretable model, while Random Forest is an ensemble model known for its robustness and accuracy.

6. Model Training and Evaluation: We trained both the Decision Tree and Random Forest models on the training data. After training, we evaluated their performance using appropriate metrics such as root mean squared error (RMSE) and coefficient of determination (R2).

7. Hyperparameter Tuning: To optimize the performance of the Random Forest model, we performed hyperparameter tuning. This involved searching for the best combination of hyperparameters using techniques such as grid search or random search.

## Results and Discussion
After training and evaluating the models, we obtained the following results:

* Decision Tree: The Decision Tree model achieved an RMSE of 72180.975 and an R2 of 0.602 on the test set. This model demonstrated moderate predictive accuracy.

* Random Forest: The Random Forest model, without hyperparameter tuning, achieved an RMSE of 50198.554 and an R2 of 0.808 on the test set. It outperformed the Decision Tree model, indicating its superior predictive power.

* Random Forest (Tuned): After performing hyperparameter tuning on the Random Forest model, we achieved further improvements. The tuned Random Forest model achieved an RMSE of 49891.839 and an R2 of 0.810 on the test set, better than the untuned version.

The results indicate that the Random Forest model, especially the tuned version, offers better predictive performance compared to the Decision Tree model.

## Conclusion
In this project, we successfully developed machine learning models to predict housing prices in California. By leveraging features such as location, size, and proximity to the ocean, the Random Forest model, especially the tuned version, demonstrated superior predictive accuracy. This project highlights the potential of machine learning techniques in the real estate domain and provides insights into housing price prediction.
