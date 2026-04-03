# Simple-Linear-Regression--Gold-Price-Prediction
Predict 22k gold rate per gram in India.

This repository contains a machine learning project that predicts the current price of 22k gold per gram in India using **Simple Linear Regression**. The model uses the **USD/INR exchange rate** as the primary feature to forecast gold prices.

### **Project Overview**
The project is designed to help users understand the relationship between currency fluctuations and precious metal rates. It includes a complete end-to-end pipeline from data collection via web scraping to a live web interface for real-time predictions.

### **Key Features**
* **Data Collection**: Automates the retrieval of historical gold rates and USD/INR exchange data using `yfinance` and web scraping with `BeautifulSoup`.
* **Machine Learning Model**: Implements a Simple Linear Regression model trained on 2024 data, optimized with `RandomizedSearchCV`.
* **Web Interface**: A user-friendly GUI built with `Gradio` where users can input the current USD/INR rate to get an instant gold price prediction.
* **Persistence**: Uses `pickle` to save and load the trained regressor and feature scaler for consistent performance without retraining.

### **Tech Stack**
* **Language**: Python
* **Libraries**: 
    * `pandas` & `numpy` for data manipulation.
    * `scikit-learn` for model training and preprocessing.
    * `matplotlib` & `seaborn` for Exploratory Data Analysis (EDA).
    * `gradio` for the web application.
    * `BeautifulSoup` & `requests` for web scraping.

### **Project Structure**
* `Gold_Price_Prediction_Simple_Linear_regression.ipynb`: The primary notebook containing data cleaning, analysis, and model training.
* `app.py`: The deployment script that launches the Gradio web interface.
* `regressor.pkl` & `scaler.pkl`: Pre-trained model and data scaler files.
* `Gold vs USDINR.csv`: The dataset used for training.

### **How to Run**
1.  **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/Gold-Price-Prediction.git
    ```
2.  **Install dependencies**:
    ```bash
    pip install pandas numpy scikit-learn gradio yfinance beautifulsoup4
    ```
3.  **Launch the App**:
    ```bash
    python app.py
    ```
    This will generate a local or public URL to access the prediction tool.
