# Food_Delivery_Time_Prediction
This project developed a machine learning model to predict food delivery times, utilizing key factors like distance, weather, and traffic.

- **Data Handling**	: pandas, numpy 
- **Visualization**	: matplotlib.pyplot, plotly.express, seaborn 
- **ML Tools**	: sklearn.model_selection, sklearn.preprocessing, sklearn.compose, sklearn.linear_model, sklearn.metrics

**✨ Data Preprocessing & Feature Engineering:**
- **Data Cleaning**: Handled 30 missing values across Weather, Traffic_Level, Time_of_Day, and Courier_Experience_yrs using the mode (for categorical) and intended mean (for numerical) imputation.
- **Outlier Removal:** 6 outliers with Delivery_Time_min greater than 116 were identified and dropped.
- **Feature Creation:** Calculated a Speed feature (Distance_km / Preparation_Time_min).
- **Feature Scaling & Encoding:** Applied StandardScaler to numerical features and OneHotEncoder to categorical features using a ColumnTransformer.

**📈 Model & Performance:**
- **Model Used :** Linear Regression 
- **Evaluation Metrics :** R^2 Score 
- **Test Set Accuracy :** 0.8415 

The final $R^2$ score of 0.8415 indicates that the model explains over 84% of the variability in food delivery time. 
