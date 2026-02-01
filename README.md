# **Nairobi Price Predictor 🏠🇰🇪**

A robust machine learning pipeline designed to estimate residential property values in Nairobi, Kenya.

## **📊 Performance at a Glance**

* **Champion Model:** Random Forest Regressor  
* **Accuracy (R² Score):** 0.82 (approx.)  
* **Avg. Error (MAPE):** **22.66%**  
* **Core Driver:** Property Type (Townhouse)

## **🛠️ The Tech Stack**

* **Language:** Python 3.x  
* **Libraries:** Scikit-Learn, Pandas, NumPy, Seaborn, Matplotlib.  
* **Techniques:** Log-Transformation, One-Hot Encoding, Grouped Median Imputation.

## **🏗️ Pipeline Features**

1. **Unit Conversion Engine:** Custom Regex logic to normalize property sizes (Acre to $m^2$).  
2. **Noise Reduction:** Automatic filtering of locations with low statistical significance (fewer than 3 entries).  
3. **Standardized Preprocessing:** Scalable ColumnTransformer for numerical and categorical features.

## **🚀 Usage**

To run a prediction, use the get\_model\_prediction function in the notebook:

Python  
\# Estimate for a 3-bed Apartment in Kilimani (150sqm)  
price \= get\_model\_prediction('Apartment', 'Kilimani', 3, 2, 150, 0\)  
print(f"KES {price:,.2f}")

