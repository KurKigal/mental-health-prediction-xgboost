# Mental Health Prediction with XGBoost

This project develops a machine learning model to predict depression risk using XGBoost classifier, achieving 93.8% accuracy on mental health survey data.

## Project Objective
To predict depression risk based on various lifestyle, academic, and professional factors using machine learning techniques for early mental health intervention.

## Dataset Information
- **Source**: Kaggle Playground Series S4E11
- **Size**: 140,700 training samples × 20 features
- **Target**: Binary classification (Depression: 0/1)
- **Features**: Demographics, lifestyle, work/study patterns, mental health indicators

## Key Features
- **Demographics**: Age, Gender, City
- **Education/Work**: Academic pressure, work pressure, CGPA, job satisfaction
- **Lifestyle**: Sleep duration, dietary habits, work/study hours
- **Mental Health**: Suicidal thoughts, family history, financial stress

## Technologies Used
```python
pandas==1.5.0
numpy==1.23.0
xgboost==1.7.0
scikit-learn==1.1.0
matplotlib==3.6.0
seaborn==0.12.0
```

## Data Preprocessing
- **Missing Value Treatment**: 
  - Categorical: Mode imputation
  - Numerical: Mean imputation
- **Encoding**: One-hot encoding for categorical variables
- **Train-Validation Split**: 80-20 ratio

## Model Performance
### XGBoost Classifier Results:
- **Accuracy**: 93.81%
- **Precision**: 
  - Class 0 (No Depression): 96%
  - Class 1 (Depression): 84%
- **Recall**:
  - Class 0: 96%
  - Class 1: 82%
- **F1-Score**: 
  - Class 0: 96%
  - Class 1: 83%

### Class Distribution:
- **No Depression (0)**: 22,986 samples (81.7%)
- **Depression (1)**: 5,154 samples (18.3%)

## Installation & Usage

### Requirements
```bash
pip install pandas numpy xgboost scikit-learn matplotlib seaborn jupyter
```

### Data Download
Download the dataset from Kaggle:
```bash
kaggle competitions download -c playground-series-s4e11
```

### Execution
```bash
jupyter notebook mental-health-prediction-xgboost-93-acc.ipynb
```

## Model Insights
- **High Accuracy**: 93.8% overall classification accuracy
- **Balanced Performance**: Good precision-recall balance for both classes
- **Feature Importance**: Work pressure, sleep patterns, and financial stress are key predictors
- **Scalable**: XGBoost handles large datasets efficiently

## Key Findings
1. **Strong Predictors**: Suicidal thoughts history, family mental illness history, and work pressure are significant indicators
2. **Lifestyle Impact**: Sleep duration and dietary habits correlate with depression risk
3. **Academic vs Professional**: Both academic and work-related stress contribute to mental health outcomes
4. **Gender Patterns**: Model captures gender-specific depression risk patterns

## Applications
- **Healthcare Screening**: Early depression risk assessment
- **Educational Support**: Student mental health monitoring
- **Workplace Wellness**: Employee mental health programs
- **Research**: Mental health epidemiology studies

## Limitations
- Based on self-reported survey data
- May not capture all depression complexity
- Requires clinical validation for real-world deployment
- Potential bias in survey responses

## Future Improvements
- Feature engineering for temporal patterns
- Ensemble methods with multiple algorithms
- Cross-validation for robust performance
- External dataset validation
- Clinical expert consultation

## Ethical Considerations
This model is intended for research and screening purposes only. Professional medical consultation is essential for any mental health diagnosis or treatment decisions.

## Developer
- **Kaggle**: [@kurkigal](https://www.kaggle.com/kurkigal)

## License
MIT License

## Contributing
Contributions welcome! Please ensure ethical guidelines are followed when working with mental health data.

---
⭐ If this project helps advance mental health research, please consider starring it!