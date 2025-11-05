# LAABAthena.lk - Vehicle Price Prediction Web Application

**Student:** Chamod Dushyantha (st20224935)  
**Course:** BSc (Hons) Software Engineering  
**Batch:** CL-BSCSD-23-67  
**University:** Cardiff Metropolitan University

## Project Overview

LAABAthena.lk is a web-based application designed to predict the prices of used vehicles in Sri Lanka using machine learning. The system provides a user-friendly interface for users to input vehicle details and receive an estimated market price, helping buyers and sellers make informed decisions.

## Features

- **User Authentication:** Secure login and registration for users.
- **Vehicle Price Prediction:** Predicts car prices based on model, year, transmission, body type, fuel type, engine capacity, mileage, and economic factors.
- **Data Visualization:** Insights and statistics about the vehicle dataset.
- **Responsive UI:** Modern, mobile-friendly design with interactive elements.
- **Admin & User Views:** Different access levels for users and administrators.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (with Swiper.js for carousels)
- **Backend:** Python (Flask)
- **Database:** MySQL (user authentication and management)
- **Machine Learning:** Scikit-learn (Random Forest Regressor)
- **Others:** Pandas, NumPy, Matplotlib, Seaborn, Pickle

## How It Works

1. **Data Preparation:** The system uses a dataset of used car prices and features, cleans and encodes the data, and trains a Random Forest model.
2. **Model Deployment:** The trained model is saved and loaded by the Flask backend to make real-time predictions.
3. **User Interaction:** Users log in, enter vehicle details, and receive a predicted price instantly.
4. **Visualization:** The app provides visual insights into the dataset and prediction results.

## Project Structure

- `app.py` - Main Flask application.
- `templates/` - HTML templates for different pages (login, home, about, vehicles, result).
- `static/` - Static files (CSS, JS, images).
- `database/carprice.sql` - SQL script for user table.
- `car price .csv` - Dataset used for training.
- `usedcarprd.ipynb` - Jupyter notebook for data analysis and model training.
- `requirements.txt` - Python dependencies.

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Set up the MySQL database using `database/carprice.sql`.
3. Train the model using `usedcarprd.ipynb` (or use the provided `randomf.pkl`).
4. Run the Flask app:
   ```bash
   python app.py
   ```
5. Access the application at `http://localhost:5000`.

## Academic Note

This project was developed as the final year submission for the BSc (Hons) Software Engineering degree at Cardiff Metropolitan University. It demonstrates the integration of machine learning with web technologies to solve real-world problems in the Sri Lankan automotive market.
