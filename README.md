📌 **File:** `sensor-dashboard/README.md`

---

```md
# Sensor Dashboard (React + Recharts)

This is a simple **Sensor Data Visualization Dashboard** built using **React** and **Recharts**.
It is inspired by the ENTS (Environmental NeTworked Sensor) platform project from UCSC OSRE.

The dashboard allows users to:
- Add sensor readings
- View sensor readings on a line chart
- Filter readings by sensor type (temperature, moisture, voltage)
- Export sensor readings as CSV

---

## Features

✅ Sensor type selection (Temperature / Moisture / Voltage)  
✅ Add new sensor readings (value + timestamp)  
✅ Interactive line chart visualization using Recharts  
✅ Fetch readings from backend Flask API  
✅ Export sensor readings as CSV  

---

## Tech Stack

- React (Frontend)
- Recharts (Charts)
- Axios (API calls)

---

## Folder Structure

```

sensor-dashboard/
│── public/
│── src/
│   │── components/
│   │   │── SensorChart.jsx
│   │   │── SensorForm.jsx
│   │
│   │── pages/
│   │   │── Dashboard.jsx
│   │
│   │── services/
│   │   │── api.js
│   │
│   │── App.js
│   │── index.js
│
│── package.json
│── README.md

````

---

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/sensor-dashboard.git
cd sensor-dashboard
````

### 2. Install dependencies

```bash
npm install
```

### 3. Start the frontend server

```bash
npm start
```

The frontend will run on:

```
http://localhost:3000
```

---

## Backend Requirement

This frontend requires a Flask backend API running at:

```
http://127.0.0.1:5000
```

backend has the following endpoints:

* `GET /api/readings?sensor=temperature`
* `POST /api/readings`
* `GET /api/readings/export/csv?sensor=temperature`

---

## CSV Export Feature

The dashboard includes a "Download CSV" button which downloads sensor data using:

```
/api/readings/export/csv?sensor=<sensorType>
```

---

## Purpose of This Project

This project is built as practice for open source contribution and OSRE/GSoC style programs.
It demonstrates:

* Frontend development in React
* API integration using Axios
* Data visualization dashboards
* CSV export functionality

---

## Future Improvements (Planned)

* Date range filtering
* Drag and drop chart layout
* Custom chart styling (color, line width)
* Save dashboard layout using URL parameters
* Authentication support


