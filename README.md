# Cinema-Audience-Forecasting-Machine-Learning-Project

#Project_Overview 
This project aims to forecast daily cinema audience attendance using historical data from online bookings and on-site ticket sales. By capturing time-series patterns, booking behavior, and calendar effects (weekends and holidays), the model predicts future audience demand for individual theatres. 

#Problem_Statement
Given historical data from online booking platforms, POS ticket sales, daily visit records, and calendar information, the objective is to predict the number of audiences attending each theatre on future dates.
 This is a challenging time-series forecasting problem with seasonality, external factors, and sparse data (including zero-audience days due to closures).

#Dataset_Summary
Data is collected from two platforms:
BookNow – Online advance bookings
CinePOS – On-site POS ticket sales
Key files include theatre metadata, booking transactions, daily visit counts, calendar features, and theatre ID mappings.

#Key_Challenges
Multiple data sources with different theatre IDs
Sparse time series with zero-audience days
Strong weekend and holiday effects
Different online vs walk-in booking behaviors

#Methodology
Data Integration: Mapped theatres across platforms and aggregated bookings at theatre–date level
Feature Engineering: Day-of-week, weekends, holidays, lag features, rolling statistics, and booking trends
Modeling: Supervised time-series forecasting using statistical and machine learning regression models
Zero-Audience Handling: Retained in training; excluded from scoring as per rules

#Evaluation
Predictions were generated for each theatre-date pair following the required submission format:

ID = book_theater_id + show_date
audience_count = predicted value

#Tools_Used
Python, Pandas, NumPy, Matplotlib, Scikit-learn, and time-series feature engineering techniques.

#Key_Insights
Strong weekly seasonality in audience attendance
Holidays and weekends significantly boost footfall
Online bookings are a leading indicator of walk-in audiences
Theatre-specific patterns improve prediction accuracy

#Future_Scope
Deep learning models (LSTM, Temporal CNN)
Movie-level features (genre, release dates)
Better modeling of theatre closures
Probabilistic forecasting for uncertainty estimation

#Conclusion
This project showcases an effective time-series forecasting pipeline using multi-source data integration and feature engineering to predict cinema audience demand, closely reflecting real-world forecasting challenges in the entertainment industry.
