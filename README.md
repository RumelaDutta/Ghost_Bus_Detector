# 🚌 Ghost Bus Detector

A real-time bus tracking and anomaly detection system that helps identify *ghost buses* (buses that appear on schedules but don’t actually arrive) and other irregularities. This project uses *FastAPI, Redis, React, and WebSockets* to fetch, process, and visualize bus data on an interactive map.

This is my *first project*, built to learn how backend, frontend, and live data pipelines work together in real-world applications.

---

## ✨ Features

* 🔴 Detect *ghost buses* in real-time
* 📡 Live bus tracking on an interactive *Leaflet map*
* 📊 *Bus trend chart* to visualize activity patterns
* ⚠ *Alerts & notifications* when anomalies occur
* 🔍 Filters to view specific buses and statuses
* 📌 Click on a bus to see detailed information

---

---

## 📂 Project Structure


Ghost-Bus-Detector/

│── backend/        # FastAPI server & Redis integration

│── frontend/       # React frontend with map and charts

│── README.md       # Project documentation


---

## ⚡ Getting Started

Follow these steps to set up and run the project locally.

### ⿡ Clone the repository

https://github.com/RumelaDutta/Ghost_Bus_Detector


### ⿢ Backend Setup (FastAPI + Redis)

1. Navigate to backend folder:

   bash
   cd backend
   

2. (Optional) Create a virtual environment:

   bash
   python -m venv venv
   
   source venv/bin/activate    # On Mac/Linux
   
   venv\Scripts\activate       # On Windows
   

4. Install dependencies:

   bash
   pip install -r requirements.txt
   

5. Start the FastAPI server:

   bash
   uvicorn main:app --reload
   

### ⿣ Frontend Setup (React)

1. Open a new terminal and go to the frontend folder:

   bash
   cd frontend
   

2. Install dependencies:

   bash
   npm install
   

3. Start the React app:

   bash
   npm start
   

---

## 🚀 How It Works

1. The backend fetches bus data using *GTFS-Realtime API*.
2. Data is processed and anomalies (ghost buses, missing buses, delays) are detected.
3. The data is stored in *Redis* and served to the frontend via *WebSockets*.
4. The React app displays buses on a *map*, along with alerts and trend charts.

---


