# 🚖 MyDriver

<div align="center">

# 🚖 MyDriver

### AI-Powered Ride-Hailing Application

A full-stack ride-hailing mobile application inspired by Uber, built with **Flutter**, **Firebase**, **FastAPI**, and **Machine Learning**.

<!-- TODO: Replace with your project banner -->
<img src="assets/banner.png" width="900">

<br>

![Flutter](https://img.shields.io/badge/Flutter-3.x-blue?logo=flutter)
![Firebase](https://img.shields.io/badge/Firebase-Firestore-orange?logo=firebase)
![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green?logo=fastapi)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-red)
![XGBoost](https://img.shields.io/badge/XGBoost-Regressor-success)

</div>

---

# 📑 Table of Contents

- [About](#-about)
- [Features](#-features)
- [Application Flow](#-application-flow)
- [Machine Learning](#-machine-learning)
- [Tech Stack](#-tech-stack)
- [Architecture](#-architecture)
- [Screenshots](#-screenshots)
- [Installation](#-installation)
- [Project Structure](#-project-structure)
- [REST API](#-rest-api)
- [Challenges](#-challenges)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

# 📖 About

MyDriver is a complete ride-hailing mobile application inspired by modern transportation platforms such as Uber.

The application enables passengers to request rides, receive offers from nearby drivers, communicate in real-time, track the driver's live location, and estimate trip duration using an AI model trained on historical taxi trip data.

The project combines multiple software engineering disciplines into one production-like application including:

- Mobile Development
- Backend Development
- Machine Learning
- Cloud Database
- Authentication
- REST APIs
- Real-time Communication
- GIS & Navigation

---

# ✨ Features

## 👤 Passenger

- User Authentication
- Edit Profile
- Live Map
- Select Pickup & Destination
- Nearby Drivers Detection
- Ride Request
- Receive Driver Offers
- Accept Driver
- Live Driver Tracking
- In-App Chat
- Trip Rating
- Estimated Trip Distance
- AI Trip Duration Prediction

---

## 🚗 Driver

- Driver Authentication
- Online / Offline Status
- Receive Ride Requests
- Accept / Reject Trips
- Live Location Updates
- Passenger Chat
- Navigation
- Complete Ride
- Receive Ratings

---

# 🔄 Application Flow

```text
Passenger

↓

Choose Destination

↓

Calculate Route

↓

Estimate Trip Duration (AI)

↓

Send Ride Request

↓

Nearby Drivers Receive Request

↓

Driver Accepts

↓

Passenger Selects Driver

↓

Trip Starts

↓

Live Tracking

↓

Trip Ends

↓

Rating
```

---

# 🤖 Machine Learning

One of the main goals of this project is integrating Machine Learning into a real-world mobile application.

The prediction model estimates trip duration before requesting a ride.

## Model

- XGBoost Regressor

---

## Feature Engineering

The following features are generated before prediction:

- Passenger Count
- Store & Forward Flag
- Trip Distance
- Month
- Hour
- Minute
- Weekend
- Day of Week
- Rush Hour
- Night Trip
- Airport Trip
- Estimated Speed
- Bearing Angle

---

## Prediction Pipeline

```text
Flutter

↓

REST API

↓

FastAPI

↓

Preprocessing

↓

Feature Engineering

↓

XGBoost Model

↓

Prediction

↓

Flutter UI
```

---

# 🛠 Tech Stack

## Mobile

- Flutter
- Dart

---

## Backend

- FastAPI
- Python

---

## Machine Learning

- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- Joblib

---

## Cloud

- Firebase Authentication
- Cloud Firestore

---

## Maps

- OpenStreetMap
- Flutter Map
- OSRM Routing API

---

## State Management

> ⚠️ TODO:
>
> Replace with your state management solution
>
> Example:
>
> Provider
>
> Riverpod
>
> Bloc

---

# 🏗 Architecture

```text
                Flutter App
                     │
      ┌──────────────┼──────────────┐
      │              │              │
      ▼              ▼              ▼

 Firebase      OpenStreetMap      FastAPI
Authentication      │              │
      │             │              ▼
      ▼             ▼        Machine Learning
 Firestore      Route API         XGBoost
      │
      ▼
 Realtime Database
```

---

# 📱 Screenshots

> ⚠️ TODO:
>
> Replace with screenshots

| Home | Driver | Chat |
|------|--------|------|
| Image | Image | Image |

| Ride | Tracking | Rating |
|------|----------|---------|
| Image | Image | Image |

---

# 🚀 Installation

Clone repository

```bash
git clone https://github.com/USERNAME/MyDriver.git
```

Go to project

```bash
cd MyDriver
```

Install packages

```bash
flutter pub get
```

Run

```bash
flutter run
```

---

## Backend

Install requirements

```bash
pip install -r requirements.txt
```

Start server

```bash
uvicorn main:app --reload
```

---

# 📂 Project Structure

```text
lib/

├── models/

├── pages/

├── widgets/

├── services/

├── assistant/

├── authentication/

├── global/

├── infoHandler/

└── main.dart

API/

├── main.py

├── predict.py

└── requirements.txt

MachineLearning/

├── dataset/

├── preprocessing/

├── feature_engineering/

├── training/

└── Model/
```

> ⚠️ Update this tree according to your project structure.

---

# 🌐 REST API

## POST /predict

Predict trip duration.

### Request

```json
{
  "passenger_count":1,
  "distance_KM":5.6,
  "hour":14,
  "minute":20,
  "month":7
}
```

### Response

```json
{
   "trip_duration": 842.6
}
```

---

# 📊 Machine Learning Performance

> ⚠️ Replace these values after training.

| Metric | Value |
|---------|------:|
| MAE | xx |
| RMSE | xx |
| R² Score | xx |

---

# ⚡ Challenges

Some interesting challenges solved during development include:

- Integrating Machine Learning with Flutter.
- Real-time driver tracking.
- Synchronizing passenger and driver states.
- Feature engineering for trip duration prediction.
- Building REST APIs using FastAPI.
- Firebase realtime synchronization.
- Route calculation using OSRM.
- Optimizing prediction accuracy.

---

# 🚀 Future Improvements

- Online Payment
- Push Notifications
- Dynamic Pricing
- Driver Earnings Dashboard
- AI Route Optimization
- ETA Prediction Enhancement
- Ride History Analytics
- Dark / Light Themes
- Admin Dashboard
- Docker Deployment

---

# 📚 What I Learned

This project helped me gain hands-on experience in:

- Flutter Development
- Firebase Services
- REST API Design
- Machine Learning Deployment
- Feature Engineering
- XGBoost Regression
- Backend Development
- Mobile UI/UX
- Clean Project Architecture
- Debugging Large Projects

---

# 🤝 Contributing

Contributions, ideas, and suggestions are welcome.

Feel free to fork the repository and submit a pull request.

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

## Waleed Raslan

Computer Science Student

Flutter Developer

Machine Learning Enthusiast

Artificial Intelligence Developer

---

<div align="center">

⭐ If you like this project, don't forget to leave a star!

</div>