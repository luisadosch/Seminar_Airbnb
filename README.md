### Project: Predicting Airbnb Prices with Machine Learning  

#### 📝 Description  
Developed a predictive model using machine learning algorithms to forecast Airbnb prices based on various features such as **location, amenities, and property type**.  

#### 🛠️ Technologies Used  
- **Python**  
- **scikit-learn**  
- **pandas**  
- **osmnx**  
- **geopandas**  

#### 🚀 Challenges  
- Handling missing data  
- Feature engineering  
- Model evaluation  

#### 🤖 Models Used  
- **Random Forest Regressor**  
- **Linear Regression**  
- **Geospatial Models** (SLX & SAR)  

#### 📊 Findings  
- **Key factors influencing property prices** include location, property size, and proximity to attractions.  
- **Spatial influences** also play a role in price predictions.  

### 🌍 Map of Airbnb Prices in Prague  
![Airbnb Prices Map](airbnb_prices.html)  

- The dots represent Airbnb listings in **Prague**. Brighter colors indicate **higher prices**.  
- As expected, the **highest prices** are concentrated in the **Old Town of Prague**.  

### 📈 Results and Model Comparison  

| Model                           | Property Features | POI Features | Spatial Lag | Spatial Cross Correlation | Relative Improvement RMSE |
|---------------------------------|------------------|--------------|-------------|-------------------------|--------------------------|
| Ordinary Least Squares Regression | ✅ | ❌ | ❌ | ❌ | 0% |
| Geospatial Regression            | ✅ | ✅ | ✅ | ✅ | 8% |
| Random Forest                    | ✅ | ❌ | ❌ | ❌ | -2% |
| Random Forest (with POIs)         | ✅ | ✅ | ❌ | ❌ | 14% |

### 📍 What are Points of Interest (POIs)?  
- **Points of Interest (POIs)** are locations that may attract people, such as **restaurants, bars, and public transportation**.  

### 🗺️ What are Spatial Lags and Spatial Cross Correlation?  
- **Spatial Lag:** Measures the influence of **neighboring properties' prices** on the price of a property. It captures **spatial autocorrelation** of property prices.  
- **Spatial Cross Correlation:** Measures the relationship between the **spatial distribution** of different variables, capturing **spatial dependence** between features.  

### 🔑 Key Findings  
- **Effect of Space:** Considering **spatial influences** improves price predictions.  
- **Best Models:** The best models are either **linear models with complex spatial features (spatial regression)** or **non-linear models (random forest) with simpler geospatial features (POIs)**.  
