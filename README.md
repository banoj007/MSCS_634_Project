# Final Insights, Recommendations, and Presentation

## 1. Project Overview
This project focuses on analyzing car price prediction using the **Car Price Assignment Dataset**. The primary goal was to understand the key factors influencing car prices and to build predictive models using regression, classification, clustering, and association rule mining techniques.

## 2. Dataset Description and Justification
The dataset, **CarPrice_Assignment.csv**, contains detailed information about various car attributes such as make, model, fuel type, engine specifications, and price.  
It was chosen because:
- It offers a rich set of numerical and categorical variables suitable for multiple data analysis methods.
- It represents a real-world scenario of automotive pricing.
- It allows exploration of regression, classification, and clustering methods in a practical context.

## 3. Data Preprocessing, EDA, and Feature Engineering
Key preprocessing steps:
- Removed duplicates and handled missing values.
- Converted categorical variables into numerical form using one-hot encoding.
- Normalized numerical features for better model performance.
- Created new engineered features like **power-to-weight ratio** and **engine size category**.

EDA Insights:
- Strong positive correlation between **engine size** and **price**.
- Luxury brands such as BMW, Audi, and Mercedes show consistently higher prices.
- Fuel type and body style influence pricing but less than engine-related features.

Feature Engineering Highlights:
- Grouped car companies into **luxury**, **mid-range**, and **economy**.
- Binned continuous features into categories for classification models.

## 4. Model Results

### Regression (Price Prediction)
- **Model Used**: Linear Regression, Random Forest Regressor
- **Best R² Score**: 0.92 (Random Forest)
- **Key Predictors**: Engine size, horsepower, curb weight, and brand.

### Classification (Price Range Prediction)
- Converted price into three categories: Low, Medium, High.
- **Best Accuracy**: 89% (Random Forest Classifier)

### Clustering
- Applied K-Means clustering on normalized features.
- Optimal clusters (k=3) correspond closely to luxury, mid-range, and economy segments.

### Association Rule Mining
- Mined frequent patterns linking car features to high/low prices.
- Example Rule: `{luxury_brand=True, engine_size>200}` → `price_category=High` (Support: 0.25, Confidence: 0.88)

## 5. Key Insights
- Engine size, horsepower, and brand reputation are the strongest determinants of price.
- There is a clear segmentation in the market: economy, mid-range, and luxury cars.
- Feature engineering improved model performance across all tasks.
- Association rules confirm brand and engine characteristics strongly align with higher price categories.

## 6. Practical Recommendations
- **For Manufacturers**: Focus marketing efforts on engine and performance specs for luxury cars, and on fuel efficiency for economy cars.
- **For Buyers**: Consider total cost of ownership, as price correlates with maintenance in high-horsepower cars.
- **For Dealers**: Use segmentation models to tailor promotions for specific buyer groups.

## 7. Ethical Considerations
- **Data Privacy**: Dataset contained no personally identifiable information.
- **Fairness**: Avoided using attributes that could lead to socio-economic discrimination.
- **Bias Mitigation**: Checked for imbalance across brands and adjusted through sampling where necessary.

## 8. Conclusion
The project successfully demonstrated the integration of regression, classification, clustering, and association rule mining techniques to analyze car prices. The results can guide automotive stakeholders in pricing strategies, marketing, and customer targeting.

---
**Author:** Banoj Kumar Jena  
**Course:** MSCS 634 – Data Structures and Analysis  
**Deliverable 4 Submission**
