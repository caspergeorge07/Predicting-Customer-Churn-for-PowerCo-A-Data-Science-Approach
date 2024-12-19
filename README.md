# **Predicting Customer Churn for PowerCo: A Data Science Approach**

## **Overview**
This project addresses customer churn for PowerCo, a gas and electricity utility serving small and medium-sized enterprises. With increasing competition in the energy market, PowerCo is seeking to understand the factors influencing churn, especially price sensitivity, to retain its customers.  

The project involves:
- Defining price sensitivity and quantifying its effect on churn.
- Preparing and engineering features from customer, churn, and historical price data.
- Developing and evaluating machine learning models to predict churn and identify key drivers.

---

## **Data Description**
Three datasets were used:
1. **Customer Data (`client_data.csv`)**:
   - Includes customer characteristics such as electricity and gas consumption, contract dates, and churn status.
   - Key fields: `cons_12m`, `forecast_cons_12m`, `margin_net_pow_ele`, `churn`.

2. **Price Data (`price_data.csv`)**:
   - Includes historical prices for electricity and gas, categorized by off-peak, peak, and mid-peak periods.
   - Key fields: `price_off_peak_var`, `price_peak_var`, `price_mid_peak_var`.

3. **Cleaned Data**:
   - Processed and merged datasets prepared for modeling.

---

## **Key Steps in the Project**
1. **Exploratory Data Analysis (EDA)**:
   - Visualized consumption patterns, price trends, and churn rates.
   - Identified correlations between price sensitivity and churn.

2. **Feature Engineering**:
   - Created features like `price_sensitivity` and forecasted margins to capture customer behavior.
   - Handled missing values, encoded categorical variables, and normalized numerical data.

3. **Model Building**:
   - Trained binary classification models (Random Forest).
   - Evaluated models based on accuracy, explainability, and complexity.

4. **Insights**:
   - Quantified the impact of price sensitivity on churn.
   - Identified customer segments at high risk of churning.

---

## **Technologies and Tools**
- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, Random Forest
- **Environment**: Jupyter Notebook  

---

## **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/powerco-churn-prediction.git
   cd powerco-churn-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebooks in the following order:
   - `Task 2 - EDA.ipynb`: Perform exploratory data analysis.
   - `Task 3 - Feature Engineering.ipynb`: Prepare and engineer features.
   - `Task 4 - Modeling.ipynb`: Train and evaluate machine learning models.

---

## **Key Results**
- **EDA Findings**:
  - Seasonal trends in energy consumption.
  - Price sensitivity significantly correlated with churn.
- **Model Performance**:
  - Random Forest achieved the highest accuracy (85%) and balanced performance.
  - Key features influencing churn include `price_peak_var`, `forecast_cons_12m`, and `margin_net_pow_ele`.

---

## **Sample Visualizations**
1. **Price Sensitivity vs Churn**:  
   *(Add relevant image link here)*

2. **Feature Importance**:  
   *(Add relevant image link here)*

---

## **Future Work**
- Incorporate time-series analysis for price trends.
- Extend the model to include customer satisfaction scores.
- Build dashboards for real-time churn prediction and monitoring.
