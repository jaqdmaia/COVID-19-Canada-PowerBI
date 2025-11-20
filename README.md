# COVID-19 Dashboard – Canada (Power BI)
**CSIS 3860 – Final Project (Winter 2025)**  
A multi-dataset Power BI report analyzing the spread, testing capacity, and demographic impact of COVID-19 across Canadian provinces.

---

## Overview
This dashboard integrates **three complementary datasets** to provide a complete, multi-layered view of the COVID-19 situation in Canada. It visualizes confirmed cases, deaths, recoveries, testing efforts, and demographic patterns using interactive and dynamic visuals.

The project combines:
- **Data engineering** (cleaning, merging, standardizing)
- **SQL Server modeling**
- **Power BI visualization & DAX measures**
- **Python/Jupyter notebook extraction from Kaggle**

---

## Datasets Used

### **1. COVID-19 Canada Dataset**  
Source: https://www.kaggle.com/datasets/jaswanthhbadvelu/canada-covid-19  
File used: `data_class.csv`  
Contains:
- Age group  
- Gender  
- Transmission type  
- Epidemiological details  

---

### **2. Novel Coronavirus 2019 Dataset – Canada**  
Source: https://www.kaggle.com/datasets/mdmahmudferdous/novel-corona-virus-2019-datasetcanada  
File used: `COVID_19_DATA_CANADA.csv`  
Contains:
- Daily Confirmed  
- Deaths  
- Recovered  
- Province-level data over time  

---

### **3. COVID-19 in Canada – Open Data**  
Source: https://www.kaggle.com/datasets/zinx1991/covid19-in-canada  
File used: `Testing_Canada.csv`  
Contains:
- Daily cumulative testing counts  
- Province-based testing metrics  

---

## Data Preparation & Processing

### ** Python / Jupyter Notebook**
- Automated Kaggle dataset download  
- Initial cleaning and inspection  

### ** SQL Server (SSMS)**
- Imported cleaned datasets  
- Created a structured relational model  
- Joined data using consistent province keys  

### ** Power BI Transformation Steps**
- Standardized province names (new field: `ProvinceGroup`)  
- Built a **Region Lookup Table** to align subregions with provinces  
- Converted date fields using correct locale settings  
- Merged testing dataset for consistent provincial grouping  

---

## DAX Measures Created
- `MaxConfirmedCases`  
- `MaxDeaths`  
- `MaxRecovered`  
- Additional aggregations for slicers, cumulative totals, and trend analysis  

---

## Visualizations Included
- **Symbol map** comparing confirmed, deaths, and recovered cases  
- **Time series (line chart)** for pandemic evolution  
- **Pie chart** for transmission types  
- **Bar chart** of cumulative tests by province  
- **Stacked bar chart** for gender × age group  
- **KPI cards**: Total confirmed, deaths, recovered  
- **Slicers**: Province, observation date  

---

## Dashboard Purpose & Insights
This dashboard enables users to:

- Compare COVID-19 impact across provinces  
- Explore demographic patterns and transmission modes  
- Understand testing behavior and gaps  
- Track how cases evolved geographically and over time  

The layout, slicers, and linked visuals support **clear storytelling** and an intuitive analytical experience.

---

## Author
Created by **Jaqueline Dutra Maia** for **CSIS 3860 – Data Visualization**, Winter 2025.

Feel free to connect on LinkedIn for questions or collaboration.
