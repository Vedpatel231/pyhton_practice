# Student Loan Data Analysis and Predictive Modeling

## Key Highlights:

###1. **Data Loading & Preliminary Analysis**:
    - Loaded dataset `student_data.csv`.
    - Utilized `describe()` and `info()` functions for an initial understanding of dataset attributes and characteristics.
    
###2. **Data Cleaning**:
    - Identified and treated missing values. For numerical attributes, missing values were replaced with the mean, while for categorical attributes, the mode was used.
    - Certain records with zero `ApplicantIncome` were updated to mean of the dataset.
    
###3. **Exploratory Data Analysis (EDA)**:
    - Visualized categorical attributes such as 'Gender', 'Married', 'Dependents', 'Education', 'Self_Employed', and 'Property_Area' using count plots.
    - Plotted histograms for numerical attributes to understand their distribution.
    
###4. **Feature Engineering**:
    - Created a new attribute, `Total_Income`, as the sum of `ApplicantIncome` and `CoapplicantIncome`.
    - Applied log transformation on skewed attributes to normalize their distribution.
    - Used correlation matrix to understand the relationships between attributes.
    - Dropped unnecessary columns post feature generation to retain only relevant predictors.
    
###5. **Data Preprocessing**:
    - Employed Label Encoding to convert categorical variables into a machine-readable format.
    - Divided the dataset into training and test datasets.

###6. **Modeling & Evaluation**:
    - Utilized various machine learning models including Logistic Regression, Decision Tree Classifier, Random Forest Classifier, and Extra Trees Classifier.
    - Calculated model accuracy and used cross-validation to mitigate any potential overfitting.
    - Conducted hyperparameter tuning for Random Forest Classifier to optimize the model.
    - Employed confusion matrices to analyze the performance of models on test data.
    
## Results:

The models showed promising results with the following accuracies:
- Logistic Regression: ~77.27% accuracy.
- Decision Tree Classifier: ~74.03% accuracy.
- Random Forest Classifier: ~77.27% accuracy.
- Extra Trees Classifier: ~75.32% accuracy.

With cross-validation, the models' performances were further evaluated to ensure robustness. 

## Visualizations:

Various plots and heatmaps were generated to gain insights from the data and to evaluate the model predictions. These visuals are pivotal for understanding the underlying patterns in the data and validating the models' performance.
