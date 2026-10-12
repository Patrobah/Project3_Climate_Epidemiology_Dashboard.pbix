# Project 3: Interactive Business Intelligence Canvas & Spatial Analytics
**Technology Stack:** Power BI Desktop • DAX (Data Analysis Expressions) • Relational Data Modeling  
**Dataset Scale:** 34,560 Distributed Environmental & Epidemiological Records  

## 📌 Project Overview
This repository showcases **Project 3**, a standalone Executive Decision-Support Dashboard designed to translate complex climate tracking parameters into real-time visual telemetry. 

While raw data tables and database rows provide secure storage, this project focuses entirely on the **User Interface and Data Analytics layer**. It establishes a native relational connection directly to a backend relational server to handle heavy visual data processing risk-free, providing public health directors and researchers with a seamless platform to monitor vector-borne anomalies.

---

## 🔗 Integrated Data Stack Context
This project is the visual front-end of a multi-tiered data engineering pipeline. To see the full architectural lifecycle of how this data was staged and structured, view the companion repositories:
*   🛢️ **Backend Database Infrastructure (Project 2):** 'https://github.com/Patrobah/Climate-Health-Database-Pipeline' displays the T-SQL scripts, `BULK INSERT` operations, and data-safe view conversions used to fuel this canvas.

---

## 🎮 Interactive Dashboard Features & Design Mechanics

The dashboard screen utilizes a highly synchronized, cross-filtering dual-axis layout built to maximize user exploration:

### 1. National Disease Distribution Chart (Y-Axis Breakdown)
*   **Visual Type:** Clustered Horizontal Bar Chart.
*   **Metrics Tracked:** Individual, independent columns for `malaria_cases` and `dengue_cases` plotted side-by-side.
*   **National Granularity:** Aggregates and ranks disease volumes across all countries.

### 2. Multi-Metric Epidemiological Timeline (X-Axis Pipeline)
*   **Visual Type:** Dual-Axis Line Chart.
*   **Primary Axis:** Monthly precipitation levels (`total_rainfall_mm`) plotting seasonal weather patterns.
*   **Secondary Axis:** Overlaid lines tracking concurrent transmission spikes (`malaria_cases` and `dengue_cases`).
*   **Time Hierarchy:** Built-in drill-down options across sequential `years` and `months`.

---

## ⚡ Live Interaction & Cross-Filtering Logic
This dashboard utilizes native relational keys to ensure that clicking an element on one chart dynamically recalculates the entire page wallpaper canvas in real time:
*   **Dynamic Shifting:** Clicking on a specific macro-region bar (such as the **East** or **West** cluster) triggers an instant canvas cross-filter. 
*   **Live Transformations:** The Line Chart immediately isolates and shifts its trend curves up or down on the fly, displaying the exact historical weather-to-pathogen correlation for that specific geographic zone alone.
*   **Scalable Framework:** Because the fields are linked to an engineered schema view, the dashboard automatically adapts if new columns or countries are layered into the source dataset. The canvas is ready to scale globally across **Country ➡️ Region ➡️ Time Series** hierarchies seamlessly.
---

## 🏁 How to Review the Project File
1. Download the **`Project3_Climate_Epidemiology_Dashboard.pbix`** file from this repository.
2. Open the file using **Power BI Desktop**.
3. Interact directly with the regional bars to watch the timeline trends dynamically recalculate.

