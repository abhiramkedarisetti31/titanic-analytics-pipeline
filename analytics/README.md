Part A: Exploratory Data Analysis - Chart Interpretations
Chart 1 (Survival Counts by Ticket Class and Sex): This chart reveals a stark contrast in survival outcomes based on gender and class. Females had overwhelmingly higher survival counts across all ticket classes compared to males. Furthermore, male casualties were heavily concentrated in the third class, highlighting a clear disadvantage for lower-class male passengers.

Chart 2 (Age Distribution by Survival Status and Sex): The age distribution indicates that surviving males generally had a lower median age than those who perished, suggesting that young boys were prioritized during the rescue. Conversely, the median age for females remains relatively consistent regardless of survival status, reinforcing that women of all ages were given priority.

Chart 3 (Fare Distribution by Pclass and Survival): This visualization demonstrates a strong positive correlation between the ticket fare paid, the passenger class, and survival. Passengers in first class who paid the highest fares survived at much greater rates. Meanwhile, the dense cluster of low-fare tickets in the third class is heavily dominated by passengers who did not survive.

Chart 4 (Survival Rate by Family Size and Ticket Class): Survival rates intersect notably with both family size and ticket class. For first and second-class passengers, having a small to moderate family size (2 to 4 members) correlates with peak survival chances. Across all classes, survival rates drop precipitously for large families exceeding four members.
Part B: Final Model Comparison Table
Model,Accuracy,Precision,Recall,F1 Score,AUC,MAE (Fare),RMSE (Fare),R²,Adjusted R²
Logistic Regression,0.7988,0.7647,0.6964,0.7289,0.8542,-,-,-,-
Decision Tree,0.8101,0.8085,0.6785,0.7378,0.8415,-,-,-,-
Random Forest,0.8212,0.7884,0.7321,0.7592,0.8655,-,-,-,-
Multivariate Linear Regression,-,-,-,-,-,19.45,34.82,0.3850,0.3812
Part C: Final Recommendation
I recommend deploying the Random Forest classifier for predicting passenger survival. It achieved the highest overall accuracy (0.8212) and the best balance of precision and recall, resulting in the highest F1 score (0.7592). Furthermore, its AUC of 0.8655 indicates a superior capability in distinguishing between the survival classes compared to the Logistic Regression and Decision Tree models. While the standalone Decision Tree offered slightly higher precision, the Random Forest ensemble is more robust against overfitting and will generalize better to unseen raw data.
