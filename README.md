## 📈 Phase 3: Interactive Business Intelligence Canvas (Power BI Deployment)

The architecture scales past database processing grids into a fully functional **Executive Decision-Support Dashboard** via Power BI Desktop. By establishing a native relational connection directly to the SQL Server view layer (`Project3_climate_epidemiology_dashboard`), the canvas visualizes complex environmental metrics without manual data transformation overhead.

### 🎮 Live Dashboard Cross-Filtering Mechanics
The production dashboard features a highly synchronized, cross-filtering dual-axis architecture:
1. **Visual #1: Regional Disease Distribution Matrix:** A horizontal Clustered Bar Chart mapping separate `malaria_cases` and `dengue_cases` distributions side-by-side. It cleanly breaks down data across different countries.
2. **Visual #2: Epidemiological Timeline Engine:** A multi-variable Dual-Axis Line Chart plotting monthly environmental anomalies (`total_rainfall_mm` on the primary axis) against moving transmission rates (`malaria_cases` and `dengue_cases` on the secondary axis).

### ⚡ Dynamic Data Synchronization (The Live Update Loop)
* **Interactive Slicing:** When a reviewer clicks on a specific country (e.g., **Kenya** or **Israel**) on the bar chart, the entire dashboard canvas reacts instantly.
* **Live Graph Transformations:** The timeline charts dynamically recalculate on the fly. The lines for Rainfall, Malaria, and Dengue automatically shift up or down, showing you the exact history for that specific region.
* **Scalable Architecture:** Because the backend is built on relational keys `(country, region, year, month)`, this dashboard is fully ready to handle new datasets. If rows are added for new countries or territories, the dashboard will scale automatically, allowing global filtering across **Country ➡️ Region ➡️ Time Series** without breaking the visualization layout.
