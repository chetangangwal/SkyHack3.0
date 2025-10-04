# ✈️ Flight Difficulty Score – United Airlines (ORD)

## Overview
This project builds a **data-driven framework** to quantify the operational complexity of flights departing from **Chicago O’Hare International Airport (ORD)**.  
Using flight-level, passenger, baggage, and station-level datasets, it calculates a **Flight Difficulty Score** that measures how challenging each flight is to manage.  
The model ranks and classifies flights daily into *Difficult*, *Medium*, and *Easy* categories, helping identify flights that require additional operational attention.

---

## 🎯 Objectives
- Compute a **Flight Difficulty Score** for each flight using multiple operational features  
- Rank flights daily to identify the most complex ones  
- Classify flights into *Difficult*, *Medium*, and *Easy* categories  
- Analyze and visualize key operational drivers (delays, ground time, baggage, etc.)  
- Provide actionable insights to improve planning and on-time performance  

---

## 🧩 Datasets
All datasets used in this project are stored in the `/data` folder:

| Dataset Name | Description |
|---------------|-------------|
| **Airports Data.csv** | Contains details of airport stations including turnaround standards and capacity metrics |
| **Bag Level Data.csv** | Provides baggage-level information such as checked and transfer bags |
| **Flight Level Data.csv** | Contains flight schedules, aircraft type, departure delays, and ground times |
| **PNR Flight Level Data.csv** | Passenger-level data per flight, including total passengers and load factors |
| **PNR Remark Level Data.csv** | Special service requests (SSR) and customer-specific needs for each booking |

---

## 📂 Repository Structure
Flight-Difficulty-Score/
│
├── Sky.ipynb # Main Jupyter Notebook with full analysis and scoring logic
├── Answer.csv # Final output with flight details, features, and difficulty score
├── data/
│ ├── Airports Data.csv
│ ├── Bag Level Data.csv
│ ├── Flight Level Data.csv
│ ├── PNR Flight Level Data.csv
│ └── PNR Remark Level Data.csv
├── presentation/
│ └── Flight_Difficulty_Score_Presentation.pptx
├── requirements.txt # Python dependencies
└── README.md # Project documentation (this file)

## ⚙️ Instructions to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/Flight-Difficulty-Score.git
   cd Flight-Difficulty-Score

2. Install required Python libraries:

        pip install -r requirements.txt

3. Open and run the Jupyter Notebook:

         jupyter notebook Sky.ipynb

4. The notebook generates Answer.csv containing:

    Flight details
    Engineered features
    Final difficulty score
    Daily ranking and classification

Key Insights

  High passenger load and baggage volume significantly contribute to delay likelihood
  Flights with shorter ground times than minimum turn minutes tend to score higher in difficulty
  Special service request (SSR) volume adds to operational complexity even after controlling for load

Tech Stack

  Language: Python
  Libraries: pandas, numpy, matplotlib, seaborn, datetime
  Tools: Jupyter Notebook, Git, GitHub

Summary

This project transforms flight operations data into actionable intelligence by quantifying flight complexity in a structured, repeatable manner — enabling proactive resource allocation and improving on-time performance at ORD.
