# 🎬 Cinema Audience Forecasting – Machine Learning Project

## 📌 Project Overview
This project focuses on forecasting **daily cinema audience attendance** using historical data from **online advance bookings** and **on-site POS ticket sales**. By leveraging **time-series patterns**, **booking behavior**, and **calendar effects** (weekends and holidays), the model predicts future audience demand for individual theatres.

---

## 🎯 Problem Statement
Given historical data from:
- Online booking platforms  
- On-site POS ticket sales  
- Daily audience visit records  
- Calendar and holiday information  

The objective is to **predict the number of audiences attending each theatre on future dates**.

This is a **time-series forecasting problem** characterized by:
- Strong seasonality  
- External calendar effects  
- Sparse data (including zero-audience days due to theatre closures)

---

## 🗂 Dataset Summary
The dataset integrates data from two platforms:
- **BookNow** – Online advance booking platform  
- **CinePOS** – On-site Point-of-Sale (POS) ticketing system  

### Key Files
- Theatre metadata  
- Booking transaction records  
- Daily visit counts  
- Calendar features (weekends, holidays)  
- Theatre ID mapping across platforms  

---

## 🔍 Key Challenges
- Multiple data sources with different theatre identifiers  
- Sparse time series with zero-audience days  
- Strong weekend and holiday effects  
- Different online vs walk-in booking behaviors  

---

## 🧠 Methodology

### Data Integration
- Mapped theatres across BookNow and CinePOS platforms  
- Aggregated booking and visit data at **theatre–date** level  

### Feature Engineering
- Day of week  
- Weekend indicator  
- Holiday flag  
- Lag features  
- Rolling statistics  
- Booking trend indicators  

### Modeling
- Framed as a **supervised time-series forecasting** problem  
- Applied statistical and machine learning regression models  

### Zero-Audience Handling
- Zero-audience days retained during training  
- Excluded from final scoring as per competition rules  

---

## 📈 Evaluation
Predictions are generated for each theatre–date pair using the following submission format:


---

## 🛠 Tools & Technologies
- Python  
- Pandas & NumPy  
- Matplotlib  
- Scikit-learn  
- Time-series feature engineering techniques  

---

## 📊 Key Insights
- Audience attendance exhibits strong weekly seasonality  
- Holidays and weekends significantly increase footfall  
- Online bookings act as a leading indicator of walk-in audiences  
- Theatre-specific patterns improve forecasting accuracy  

---

## 🚀 Future Scope
- Deep learning models (LSTM, Temporal CNN)  
- Incorporation of movie-level metadata (genre, release dates)  
- Improved handling of theatre closures  
- Probabilistic forecasting for uncertainty estimation  

---

## 🧾 Conclusion
This project demonstrates an effective **time-series forecasting pipeline** using multi-source data integration and feature engineering to predict cinema audience demand. The approach closely mirrors real-world demand forecasting challenges in the entertainment industry.

---

## 📜 License
This project is for educational and research purposes.


