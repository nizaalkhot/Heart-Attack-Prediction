## About Dataset

### Dataset Description

This dataset focuses on "Heart Attack in Youth vs. Adults in Indonesia (Statewise)" and is designed for exploratory data analysis, machine learning, and public health research. The dataset contains simulated data of 170,501 individuals from various Indonesian states, providing a comprehensive view of the factors contributing to heart attack incidents among youth (15–40 years) and adults (41–65 years). The dataset aims to help understand demographic, lifestyle, environmental, and health-related trends.

### Context and Inspiration

Heart disease remains one of the leading causes of death worldwide. By examining data from Indonesia—a diverse country with varying socio-economic, environmental, and healthcare access factors—we can uncover trends that can inform prevention strategies. The data reflects real-world unevenness and variability to simulate complex relationships, such as the interplay between age, lifestyle, environmental conditions, and medical history.

### Sources

- Simulated based on publicly available trends in health data.
- Inspired by global health datasets and studies on heart attack risk factors.
- Includes state-level diversity and unique conditions of Indonesia.

### Analysis and Prediction Workflow

#### Data Analysis
- **Loading and Exploring the Dataset**: The dataset contains 25 columns, including demographic, health, and environmental features. Key columns include `Age`, `Gender`, `Cholesterol`, `SmokingHabits`, `PhysicalActivity`, `BMI`, `Hypertension`, and `HeartAttack` (target variable).
- **Handling Missing Values**: Checked for missing data; the dataset has no missing values, ensuring completeness.
- **Encoding Categorical Variables**: Used `LabelEncoder` to transform categorical variables into numerical format.
- **Scaling Numerical Features**: Standardized numerical columns such as `Age`, `BMI`, and `Cholesterol` for better model performance.

#### Prediction Model
- **Model Selection**: Built a predictive model using a Random Forest Classifier to classify individuals as likely to have a heart attack (Yes/No).
- **Data Splitting**: Split the data into 80% training and 20% testing subsets to ensure reliable evaluation.
- **Model Training**: Trained the Random Forest model on the training data with hyperparameters tuned for optimal performance.
- **Model Evaluation**: Achieved high accuracy on the test set, with performance metrics including precision, recall, and F1-score calculated to assess model effectiveness.
- **Confusion Matrix**: Visualized the confusion matrix to understand prediction strengths and weaknesses.

#### Outputs
- **Accuracy**: The model demonstrated robust predictive performance.
- **Saved Artifacts**: The trained model, label encoders, and scaler are saved for future use.

### Files
- **heart_attack_prediction_model.pkl**: Trained Random Forest model.
- **label_encoders.pkl**: Encoders for categorical features.
- **scaler.pkl**: StandardScaler for numerical data preprocessing.

### Future Work
- Explore advanced models like Gradient Boosting or Neural Networks.
- Perform feature importance analysis to identify key predictors.
- Investigate correlations between demographic and lifestyle factors and heart attack incidence.