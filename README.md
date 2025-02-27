# 🌦️ Real-Time-Weather-Forecasting 

A machine learning-based **Weather Prediction System** that integrates **real-time weather data** from OpenWeatherMap with **historical data** to forecast **temperature, humidity, and rainfall probabilities**.  

## **📌 Features**  
✅ Fetches **current weather data** from OpenWeatherMap API 🌍  
✅ Loads **historical weather records** from `weather.csv` 📊  
✅ Uses **Random Forest Classifier** to predict if it will rain tomorrow ☔  
✅ Uses **Random Forest Regressor** to forecast temperature & humidity 🌡️  
✅ Provides **detailed weather insights** for better decision-making 📈  

---

## **⚙️ How It Works?**  
The project follows a **structured workflow** combining **real-time data, historical data, and machine learning** to provide accurate weather predictions.  

### **1️⃣ Fetch Live Weather Data**  
- Users enter a **city name**.  
- The system **fetches live weather data** from OpenWeatherMap API.  
- Includes **temperature, humidity, wind speed, pressure, and weather conditions**.  

### **2️⃣ Load Historical Weather Data**  
- Reads past weather data from `weather.csv`.  
- Cleans and pre-processes the dataset.  
- Extracts key parameters like **temperature, humidity, wind speed, pressure, and rainfall records**.  

### **3️⃣ Train Machine Learning Models**  
🔹 **Rain Prediction Model (Classification)**  
- **Model**: Random Forest Classifier  
- **Goal**: Predict whether it will rain tomorrow based on historical weather conditions.  

🔹 **Temperature & Humidity Prediction Model (Regression)**  
- **Model**: Random Forest Regressor  
- **Goal**: Forecast temperature & humidity levels for the next few hours.  

### **4️⃣ Make Predictions**  
- Predicts **rainfall probability for tomorrow**.  
- Forecasts **temperature & humidity for the next 5 hours**.  

### **5️⃣ Display Results**  
- **Current weather** (from API)  
- **Past trends** (from historical data)  
- **Future predictions** (from ML models)  

---

## **📌 Why Use Both Real-Time & Historical Data?**  
Using **both** live weather data and historical records improves **prediction accuracy**:  
✅ **Live Data** – Ensures **up-to-date** weather conditions.  
✅ **Historical Data** – Helps **train ML models** for better forecasts.  
✅ **Combination** – Provides **reliable and adaptive weather predictions**.  

---

## **🔧 Installation & Setup**  
### **Prerequisites**  
Ensure you have the following installed:  
- Python 3.x  
- Jupyter Notebook or any Python IDE  
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `requests`  

## Installation & Setup  
Clone the repository using `git clone https://github.com/your-username/weather-prediction.git` and navigate into the project directory using `cd weather-prediction`. Install dependencies by running `pip install -r requirements.txt`. Obtain an API Key from **[OpenWeatherMap](https://home.openweathermap.org/users/sign_up)** and replace `API_KEY = "your_api_key"` in the script. Finally, run the project using `python weather.py`.  

## How It Works  
The project fetches **current weather data** from OpenWeatherMap API, retrieving real-time temperature, humidity, wind speed, and weather descriptions based on user input. It then loads **historical weather data** from `weather.csv`, which contains past weather records, cleans the dataset, and prepares it for machine learning. Using a **Random Forest Classifier**, it predicts whether it will rain tomorrow based on historical trends. A **Random Forest Regressor** is then used to forecast temperature and humidity for the next 5 hours. Finally, all results, including rain predictions, temperature forecasts, and wind directions, are displayed in a structured and user-friendly format.  

## Requirements  
Python 3.x is required, along with an OpenWeatherMap API Key and necessary libraries installed via `requirements.txt`.  

## Notes  
Ensure `weather.csv` is present in the project directory. Predictions depend on the quality and quantity of historical weather data. Wind direction is converted into a readable **compass format** for better understanding.  

## License  
This project is open-source and available under the **MIT License**.  
