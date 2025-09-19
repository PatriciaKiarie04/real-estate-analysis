# real-estate-analysis

# Real Estate Data Analysis – README  

This notebook walks through the process of analyzing a real estate dataset step by step. The goal is to clean the data, explore it, and build useful visualizations to understand the factors influencing housing prices.  

---

## Step 1: Importing Libraries  
We started by importing the main Python libraries needed for data analysis and visualization:  
- **pandas** – for handling and cleaning the dataset.  
- **numpy** – for numerical computations.  
- **matplotlib** and **seaborn** – for creating plots and graphs.  

---

## Step 2: Loading the Dataset  
We loaded the real estate dataset into a pandas DataFrame (`df`). This dataset includes information such as:  
- `transaction_date` – the year and month of the transaction.  
- `house_age` – the age of the house (in years).  
- `mrt_distance` – distance to the nearest MRT (subway) station.  
- `convenience_stores` – number of nearby convenience stores.  
- `latitude` and `longitude` – location coordinates.  
- `price_per_unit` – the housing price per unit area.  

---

## Step 3: Data Cleaning  
We performed several cleaning steps:  
- Checked for **missing values**.  
- Verified **data types** (e.g., numbers vs. dates).  
- Renamed columns where necessary for clarity.  
- Created a new column `price_per_unit` to standardize the housing price information.  

---

## Step 4: Exploratory Data Analysis (EDA)  
We generated summary statistics using `.describe()` to get an overview of the dataset (mean, median, min, max, etc.). This gave us insights into the price range, house ages, and MRT distances.  

---

## Step 5: Visualizations  

### 5.1 Distribution of Housing Prices  
We plotted the distribution of `price_per_unit` to see how housing prices are spread.  

### 5.2 Price vs. House Age  
We created a scatter plot to check if older houses tend to be cheaper or more expensive.  

### 5.3 Price vs. MRT Distance  
We plotted housing prices against `mrt_distance`. This helped us see whether houses closer to MRT stations are more expensive.  

### 5.4 Price vs. Number of Convenience Stores  
We analyzed how the availability of convenience stores in the neighborhood affects housing prices.  

### 5.5 Price vs. Geographic Coordinates (Latitude / Longitude)  
Since our dataset did not contain city names or neighborhood labels, we used **latitude and longitude as a proxy for location**.  
- We identified the **top 10 most common latitudes or longitudes**.  
- Then we plotted boxplots to compare price variations across these areas.  

---

## Step 6: Insights  
From our analysis, we can draw some preliminary insights:  
1. **Proximity to MRT stations** often increases housing prices.  
2. **Houses closer to amenities (convenience stores)** tend to be valued higher.  
3. **Geographic location (latitude/longitude)** significantly influences prices – some regions are clearly more expensive than others.  
4. **House age** has a mixed effect – very old houses are cheaper, but moderately aged houses may still be valuable depending on location.  

---

## Conclusion  
We successfully:  
- Loaded and cleaned the real estate dataset.  
- Explored the main features.  
- Created visualizations to analyze how price varies with age, transport access, amenities, and location.  

This provides a solid foundation for more advanced analysis such as **predictive modeling** (e.g., regression models to forecast house prices).  

---


