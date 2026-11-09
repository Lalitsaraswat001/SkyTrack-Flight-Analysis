# ✈️ SkyTrack – Flight & Airport Analysis

An exploratory data analysis of 1,000 flight records using **R Programming**, created for the *Data Science Toolbox: R Programming (INT232)* course at Lovely Professional University.

The project cleans the data, analyses airline performance, airport traffic, flight status and delays, and presents the results with charts, tables and an R Markdown report.

> **Note:** The dataset contains simulated flight records. The findings are for academic practice and do not represent real airline performance.

---

## 📁 Files in this repository

| File | Description |
|---|---|
| `SkyTrack.Rmd` | Main R Markdown analysis (import, EDA, cleaning, visualisation, insights) |
| `SkyTrack.html` | Knitted HTML report with all outputs and charts |
| `flights-1000.csv` | Dataset (1,000 rows, 11 columns) |
| `sky.R` | Helper script for installing packages |
| `SkyTrack_Dashboard.Rmd` | Interactive dashboard (flexdashboard) *(include only if uploaded)* |

---

## 📊 Dataset

The file `flights-1000.csv` has 1,000 records and 11 columns:

`flight_id`, `flight_date`, `airline`, `origin`, `destination`, `scheduled_dep`, `actual_dep`, `dep_delay_min`, `arr_delay_min`, `distance_km`, `status`

- Period covered: 1 January 2026 – 28 August 2026
- 8 airlines and 16 airports
- 21 values are missing in `actual_dep`, `dep_delay_min` and `arr_delay_min`. These are the 21 cancelled flights, which never departed.
- No duplicate rows

---

## 🔍 What the project covers

1. Data import and inspection
2. Missing value and duplicate checks
3. Data cleaning (data types, new `month` and `weekday` columns)
4. Flight status distribution
5. Airline-wise flight counts and delay comparison
6. Top 10 busiest origin airports
7. Monthly flight trends
8. Summary statistics and key insights

---

## 📈 Key findings

- **64.1%** of flights were on time, **33.2%** delayed, **2.1%** cancelled and **0.6%** diverted.
- Average departure delay is **24.80 minutes** and average arrival delay is **22.47 minutes**. The median delay is only 6 minutes, so a few very long delays raise the average.
- **Blue Yonder** operated the most flights (148) and had the lowest average departure delay (21.54 min). **Adventure Works Air** had the highest (27.74 min).
- **Phoenix (PHX)** is the busiest origin airport with 74 departures.
- Monthly activity is stable at roughly 115–130 flights per month. August is lower because the data ends on 28 August.

---

## 🛠️ Tools and packages

R · RStudio · R Markdown · `dplyr` · `tidyr` · `lubridate` · `ggplot2` · `plotly` · `DT` · `knitr` · `readr`

---

## ▶️ How to run

1. Download or clone this repository.
2. Keep `SkyTrack.Rmd` and `flights-1000.csv` in the **same folder**.
3. Open `SkyTrack.Rmd` in RStudio.
4. Click **Knit** to generate the HTML report. Missing packages are installed automatically on the first run.

To run the dashboard (if included), open `SkyTrack_Dashboard.Rmd` and click **Knit** in the same way.

---

## 🌐 Live report

[View the report here](#) *(add your GitHub Pages link after enabling Pages)*

---

## 👤 Author

**Lalit Kumar Saraswat**
Registration No.: 62600510
Non-Degree Programme Scholarship & N2, Lovely Professional University

Guided by **Dr. Aarti** (UID: 25209), Assistant Professor, Lovely School of Computer Science and Engineering.
