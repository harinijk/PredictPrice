# Laptop Price Prediction and Classification

This project explores machine learning and deep learning techniques for analyzing laptop specifications, predicting laptop prices, and classifying laptop brands using PyTorch, NumPy, and exploratory data analysis.

The project uses regression and classification models to understand how hardware specifications such as RAM, storage, screen size, SSD usage, and touch support affect laptop pricing and brand prediction.

---

## Dataset

Dataset used:
- `laptopdata.csv`

The dataset contains laptop information including:
- Brand
- RAM
- Storage
- Storage type
- Screen size
- Touch support
- Final Price

Additional engineered features:
- `is_apple`
- `is_touch`
- `is_ssd`

---

## Project Sections

### 1. Data Preprocessing
- Loaded and cleaned laptop dataset
- Removed missing values
- Created engineered binary features
- Normalized numerical columns
- Prepared data for machine learning models

---

### 2. Exploratory Data Analysis

Visualizations included:
- Laptop price distribution
- Correlation heatmaps
- RAM vs price relationships
- Storage vs price relationships

The analysis explored how hardware specifications correlate with final laptop prices.

---

### 3. Linear Regression Models

#### Model 1 — Single Variable Regression
Predicted laptop prices using:
- Storage capacity only

Implemented manually in PyTorch using:
- gradient descent
- mean squared error loss

Metrics:
- MSE
- R² score

---

#### Model 2 — Multiple Linear Regression
Predicted laptop prices using:
- RAM
- Screen size
- SSD usage

Features:
- 5-fold cross validation
- manual gradient descent optimization
- regression equation generation
- model coefficient interpretation

---

### 4. Residual Analysis

Compared:
- actual vs predicted prices
- Apple vs non-Apple laptop residuals

This section analyzed:
- prediction bias
- model performance across brands
- pricing trends

---

### 5. Logistic Regression Classification

Built a binary classifier to predict whether a laptop is:
- Apple
- Non-Apple

Features used:
- RAM
- Storage
- SSD usage
- Touch support
- Final Price

Implemented manually using:
- sigmoid activation
- binary cross entropy loss
- gradient descent optimization

Metrics:
- accuracy
- precision

---

### Feature Engineering

Created polynomial and interaction features including:
- RAM × Storage
- RAM × Screen
- Storage × Screen
- RAM²
- Storage²
- Screen²

A nonlinear regression model was then trained using engineered features to improve price prediction performance.

---

## Technologies Used

- Python
- PyTorch
- pandas
- NumPy
- matplotlib
- seaborn

---

## Machine Learning Concepts Used

- Linear Regression
- Multiple Linear Regression
- Logistic Regression
- Gradient Descent
- Binary Cross Entropy Loss
- Feature Engineering
- Data Normalization
- Cross Validation
- Residual Analysis

---

## Results

The project demonstrated:
- strong relationships between hardware specifications and laptop prices
- improved regression performance using engineered nonlinear features
- the effectiveness of gradient descent optimization implemented from scratch
- meaningful pricing differences between Apple and non-Apple laptops

The nonlinear feature engineering model achieved better prediction performance compared to the simpler linear regression models.

