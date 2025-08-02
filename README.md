# Heart Disease Prediction Model 🫀

A comprehensive machine learning project for predicting cardiovascular disease using clinical data from Cleveland and Hungary heart disease datasets.

## 📋 Project Overview

This project implements and compares machine learning models to predict the presence of heart disease in patients based on various clinical features. The analysis includes extensive data preprocessing, exploratory data analysis (EDA), model training, evaluation, and an interactive Shiny web application for real-time predictions.

## 🏆 Key Results

- **Random Forest Model**: 92.4% accuracy
- **Logistic Regression Model**: 82.8% accuracy
- **Best Performing Model**: Random Forest with 100 trees

## 📊 Dataset

The project uses the `heart_statlog_cleveland_hungary_final.csv` dataset which combines heart disease data from Cleveland and Hungary medical institutions. The dataset includes:

- **Target Variable**: Presence of heart disease (0 = No, 1 = Yes)
- **Features**: 11 clinical attributes including:
  - Age, sex, chest pain type
  - Resting blood pressure, cholesterol levels
  - Fasting blood sugar, resting ECG results
  - Maximum heart rate achieved
  - Exercise-induced angina
  - ST depression and ST slope

## 🔬 Methodology

### Data Preprocessing
- ✅ Missing value analysis and handling
- ✅ Feature engineering and type conversion
- ✅ Data normalization (z-score scaling)
- ✅ 80/20 train-test split

### Exploratory Data Analysis
- 📈 Target variable distribution analysis
- 📊 Correlation heatmaps
- 📉 Density plots and box plots by target groups
- 🏷️ Categorical variable analysis

### Machine Learning Models
1. **Logistic Regression**
   - Baseline linear model
   - 82.8% accuracy
   
2. **Random Forest**
   - Ensemble method with 100 trees
   - 92.4% accuracy
   - Feature importance analysis

## 🛠️ Technologies Used

- **R Programming Language**
- **Libraries**:
  - `randomForest` - Random Forest implementation
  - `dplyr`, `tidyr` - Data manipulation
  - `ggplot2`, `GGally` - Data visualization
  - `corrplot`, `ggcorrplot` - Correlation analysis
  - `shiny` - Interactive web application
  - `readr` - Data import

## 📁 Project Structure

```
├── rf_model & Prototype.Rmd     # Main analysis notebook
├── heart_statlog_cleveland_hungary_final.csv  # Primary dataset
├── Heart_disease_statlog.csv    # Additional dataset
├── rf_model.rds                 # Saved Random Forest model
├── MLProjectFile.Rproj          # R project file
├── Report.pdf                   # Project report
├── Workings.pdf                 # Working documents
└── README.md                    # Project documentation
```

## 🚀 Getting Started

### Prerequisites
```r
install.packages(c("randomForest", "dplyr", "tidyr", "ggplot2", 
                   "GGally", "ggcorrplot", "corrplot", "reshape2", 
                   "patchwork", "shiny", "readr"))
```

### Running the Analysis
1. Clone this repository
2. Open the R project file (`MLProjectFile.Rproj`)
3. Run the R Markdown file (`rf_model & Prototype.Rmd`)

### Using the Saved Model
```r
# Load the pre-trained model
rf_model <- readRDS("rf_model.rds")

# Make predictions (ensure your data has the same structure)
predictions <- predict(rf_model, newdata = your_data)
```

## 📈 Model Performance

| Model | Accuracy | Notes |
|-------|----------|-------|
| Logistic Regression | 82.8% | Baseline linear model |
| Random Forest | 92.4% | Best performing model |

## 🎯 Key Features

- **Comprehensive EDA**: Detailed exploratory analysis with multiple visualization techniques
- **Model Comparison**: Side-by-side comparison of different ML algorithms
- **Feature Importance**: Analysis of which clinical factors are most predictive
- **Interactive App**: Shiny application for real-time heart disease prediction
- **Reproducible Research**: Well-documented code with proper seed setting

## 📝 Usage

This model can be used by healthcare professionals as a supplementary tool for:
- Early screening of cardiovascular disease risk
- Clinical decision support
- Research in cardiovascular health patterns

**⚠️ Disclaimer**: This model is for educational and research purposes only. It should not be used as a substitute for professional medical diagnosis.

## 👨‍💻 Author

**MD Wahid Islam Arefin**
- GitHub: [@Wahid-Islam](https://github.com/Wahid-Islam)
- Email: mdwahidislamarefin@gmail.com

## 📅 Project Timeline

- **Date Created**: May 21, 2025

## 🤝 Contributing

Feel free to fork this project, submit pull requests, or suggest improvements. All contributions are welcome!

## 📄 License

This project is available for educational and research purposes. Please cite appropriately if used in academic work.

---


*This project demonstrates the application of machine learning techniques in healthcare analytics, specifically for cardiovascular disease prediction.*
