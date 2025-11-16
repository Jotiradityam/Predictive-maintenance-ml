# Predictive Maintenance Using Machine Learning
### AI4I 2020 Industrial Equipment Dataset

## Project Overview
This project uses machine learning to predict equipment failures using the AI4I 2020 Predictive Maintenance dataset.  
A Random Forest model was trained using sensor readings and operational data, achieving 99.5% accuracy.  
The project demonstrates the application of Industrial Engineering, Machine Learning, and Smart Manufacturing.

## Dataset Information
The dataset contains 10,000 samples with the following features:

- Air temperature (K)
- Process temperature (K)
- Rotational speed (rpm)
- Torque (Nm)
- Tool wear (min)
- Machine type (L, M, H)
- Failure type indicators
- Target: Machine Failure (0 or 1)

The dataset has no missing values.

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Google Colab

## Methodology

### 1. Data Preprocessing
- Removed ID columns
- One-hot encoded machine type
- Performed 80/20 train-test split
- Handled class imbalance using class weights

### 2. Model Training
A Random Forest Classifier was used:
RandomForestClassifier( n_estimators=300, class_weight="balanced", random_state=42 )
## Results
- Accuracy: 99.5%
- Only 3 failure cases misclassified in the test set

### Classification Metrics
- Precision: 0.98
- Recall: 0.98
- F1 Score: 0.99

### Top Important Features
1. Rotational speed (rpm)
2. Torque (Nm)
3. Power Failure (PWF)
4. Heat Dissipation Failure (HDF)
5. Tool wear (min)

## Conclusion
The model effectively predicts machine failures and supports predictive maintenance strategies, helping reduce downtime and improve reliability in manufacturing.

## Future Improvements
- Build a real-time monitoring dashboard
- Deploy model using Flask/FastAPI
- Integrate with IoT sensors
- Use time-series models like LSTM

## Author
Jotiraditya Mane  
Mechanical Engineering Student
