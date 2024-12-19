# Canadian-Freight-Analysis

## **Project Overview**  

This project analyzes the Canadian Freight Analysis Framework (CFAF) dataset to uncover patterns and trends in freight transportation across Canada. The aim is to provide actionable insights into how shipment characteristics like weight, distance, commodity type, and transportation mode affect revenue generation. The project uses statistical and machine learning techniques, including Multiple Linear Regression (MLR) and interaction modeling, to guide data-driven decisions in optimizing freight operations.

## **Motivation**  

Freight transportation is critical to Canada’s economy, connecting industries, regions, and people. This project helps:  
- Identify factors influencing revenue generation.  
- Improve operational efficiency and reliability.  
- Support new freight business owners in making strategic decisions.  

## **Dataset**  

The CFAF dataset integrates data from various sources, including Statistics Canada surveys. It provides detailed information on:  
- Shipment value and weight.  
- Transportation mode (truck, rail, air, etc.).  
- Origin and destination regions.  
- Revenue generated.  

**Key Statistics:**  
- Time period: 2011 - 2017  
- Rows: ~58,721  
- Columns: Shipment details (e.g., Mode, Weight, Revenue, Distance, etc.)  

## **Objectives**  

### **Data Cleaning**  

- Handle missing values and transform categorical data.  
- Group origin and destination provinces into regions (East, West, and Other Parts).  

### **Descriptive Analysis**  
- Analyze revenue trends by mode of transport, region, and shipment characteristics.  

### **Revenue Prediction**  
- Build an MLR model to predict revenue based on shipment attributes.  
- Explore interaction effects among variables.  

### **Insights**  
- Provide recommendations for optimizing revenue generation in freight transportation.  

## **Methodology**  

### **Data Preprocessing**  

- Removed irrelevant columns (e.g., Year, TonneKm).  
- Encoded categorical variables.  
- Created new grouped columns (e.g., regions and commodity types).  

### **Exploratory Data Analysis (EDA)**  

- Visualized revenue distribution by transport modes and regions.  
- Examined relationships between revenue, weight, and distance.  

### **Modeling**  

- Built additive MLR and interaction models.  
- Evaluated models using metrics like Adjusted R-squared and Variance Inflation Factor (VIF).  

### **Model Refinement**  

- Used stepwise regression and subset selection methods to improve performance.  

## **Key Findings**  

- **Mode of Transport:** Trucks generate the highest revenue, followed by rail and air.  
- **Regions:** West Canada contributes the most to revenue, closely followed by East Canada.  
- **Distance & Weight:** Revenue increases with both shipment weight and distance traveled.  
- **Interaction Effects:** Incorporating interactions among variables significantly improves model accuracy, explaining ~91.88% of revenue variability.  

## **Tools & Libraries**  

**Programming Language:** R  

**Key Libraries:**  

- **dplyr:** Data manipulation.  
- **car:** Regression diagnostics.  
- **olsrr:** OLS regression analysis.  
- **leaps:** Model selection.  
- **GGally:** Visualization.  

## **Results**  

### **Additive Model**  
- Adjusted R-squared: 0.8017  
- Equation includes factors like transportation mode, shipment weight, distance, and commodity type.  

### **Interaction Model**  

- Adjusted R-squared: 0.9188  
- Considers interactions between numerical and categorical variables for improved predictions.  

## **Future Work**  

- Incorporate additional datasets to improve prediction accuracy.  
- Explore advanced machine learning techniques for non-linear relationships.  
- Investigate sustainability metrics in freight transportation.  
