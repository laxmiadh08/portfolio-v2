---
layout: default

permalink: /projects/environmental-health/
---
<style> 
.page-header{
    display:none;
}
.project-header { background-image: url("/images/env-health/home.png"); background-size: cover; background-position: center; 
height: 280px;
width:100%;
border-radius: 10px; margin-bottom: 25px; 
position: relative; }
.back-home { display: inline-block;
 margin: 20px 0; 
 padding: 10px 16px; 
  background: #FF7B00;
color: #ffffff;
color: white; text-decoration: none; border-radius: 6px; font-weight: bold; } 


</style>


<a class="back-home" href="/">← Back to Home</a>

<div class="project-header"></div>

# Environmental Health Monitoring Dashboard

A real-time environmental analytics system integrating weather and air quality data to monitor health risks across regions.

---

## Overview
This project collects and processes environmental data from APIs and visualizes it through an interactive dashboard.

---

## Key Features
- Real-time weather data ingestion
- Air quality index (AQI) monitoring
- Location-based environmental insights
- Historical trend tracking
- Interactive visual dashboard

---

## Tech Stack
- Python
- Dash / Plotly
- PostgreSQL
- SQLAlchemy
- Open-Meteo API

---

## Architecture
Data is fetched from APIs → ETL pipeline → PostgreSQL → Dash visualization

---

## Screenshots

![Dashboard](/assets/images/env-dashboard.png)

---

## Back to Home
[← Return Home](/)