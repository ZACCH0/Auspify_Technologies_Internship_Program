# 🎬 Netflix Content Analytics

### Auspify Technologies Internship Program | Data Analytics

**Turning raw content metadata into structured insights using Microsoft Excel, Power Query, PivotTables, PivotCharts, and interactive dashboards.**

**[INSERT IMAGE HERE — Auspify Technologies logo]**
[

---

## 📌 Project Overview

This project was completed as part of the **Auspify Technologies Internship Program**.

The objective was to transform a raw Netflix content dataset into a structured analytical solution using Microsoft Excel.

The project covers the complete workflow:

**Raw Data → Data Cleaning → Validation → Analysis → Visualization → Dashboard → Insights**

The analysis focuses on:

* Content type distribution
* Country-wise content distribution
* Release-year trends
* Audience ratings
* Content categories
* Executive-level catalog insights

---

## 🎯 Business Objective

The project was designed to answer practical questions about the structure and characteristics of the content catalog.

### Key questions

* What is the distribution between Movies and TV Shows?
* Which countries have the largest number of titles?
* How does content volume vary across release years?
* Which audience ratings are most common?
* Which content categories occur most frequently?
* How can these findings be presented in an interactive dashboard?

---

## 📂 Dataset

The dataset contains **8,790 records** and 10 fields describing Movies and TV Shows.

| Field          | Description                       |
| -------------- | --------------------------------- |
| `show_id`      | Unique content identifier         |
| `type`         | Movie or TV Show                  |
| `title`        | Content title                     |
| `director`     | Director information              |
| `country`      | Country information               |
| `date_added`   | Date added to the catalog         |
| `release_year` | Original release year             |
| `rating`       | Audience/content rating           |
| `duration`     | Movie duration or TV-show seasons |
| `listed_in`    | Content categories                |

---

# 🧹 Data Cleaning & Preparation

The raw dataset was imported and reviewed using **Power Query** before analysis.

### Cleaning and validation included:

* Checking column data types
* Reviewing categorical values
* Investigating missing/unknown values
* Checking duplicate records
* Validating dates
* Checking title formatting
* Reviewing release years
* Checking Movie/TV Show duration consistency
* Investigating structurally misaligned records

### 🔎 Data Import Issue

During the Power Query inspection, an embedded line break within a title caused one record to be incorrectly interpreted across multiple columns.

This was identified through column-level validation rather than being accepted as a normal value.

The affected record was investigated and corrected before continuing with the analysis.

**[INSERT IMAGE HERE — `type_in_power_Query.png` showing the incorrect `William Wyler` value]**
[erro]

This was an important part of the project because it demonstrated that **data validation must happen before visualization**.

---

# 📊 Task 1 — Data Cleaning & Chart Preparation

The first analytical stage established the basic structure of the dataset using PivotTables.

### Analysis included:

* Content type
* Content categories
* Country distribution
* Release year
* Rating
* Date/month distribution

### Content Type

| Type      |    Titles |
| --------- | --------: |
| Movie     |     6,126 |
| TV Show   |     2,664 |
| **Total** | **8,790** |

**[INSERT IMAGE HERE — `TASK1_Data_Cleaning_&_Chart_Preparation.png`]**

This stage provided the foundation for the subsequent dashboards.

---

# 🌍 Task 3 — Country-Wise Content Analysis

This dashboard examines how titles are distributed across countries.

### Key finding

The **United States** has the largest representation in the dataset's country field, with **3,240 titles**.

Other highly represented countries include:

* India
* United Kingdom
* Pakistan
* Canada
* Japan
* South Korea
* France
* Spain

### Analysis structure

**Rows:** Country
**Columns:** Content Type
**Values:** Count of `show_id`

Interactive filtering was also added to allow users to explore the data by content type and release year.

**[INSERT IMAGE HERE — `TASK3_Country-Wise_Content_Analysis_Dashboard.png`]**

> **Data note:** The `country` field is treated as catalog metadata. It should not automatically be interpreted as exclusive production location.

---

# 📅 Task 4 — Release Trend Analysis

This analysis examines how the number of titles varies by release year.

### PivotTable structure

**Rows:** `release_year`
**Columns:** `type`
**Values:** Count of `show_id`

### Key findings

* Content volume increases considerably across the later years represented in the dataset.
* **2018** records the highest total in the displayed release-year analysis: **1,146 titles**.
* Movies reach their highest displayed yearly count in **2018**, with **767 titles**.
* TV Shows reach their highest displayed yearly count in **2020**, with **436 titles**.
* Movies exceed TV Shows in most displayed years, although TV Shows exceed Movies in **2021**.

**[INSERT IMAGE HERE — `TASK4_Netflix_Release_Trend_Visualization.png`]**

### Data completeness note

The release-year PivotTable represents **8,009 records**, compared with the overall dataset total of 8,790. Therefore, the release-year analysis should be interpreted based on the records represented in that field.

---

# 🔞 Task 5 — Audience Rating Analysis

This dashboard examines how titles are distributed across audience/content ratings.

### Key finding

**TV-MA is the most common rating, with 3,205 titles.**

Breakdown:

* Movies: 2,062
* TV Shows: 1,143

Other major rating categories include:

| Rating | Titles |
| ------ | -----: |
| TV-MA  |  3,205 |
| TV-14  |  2,157 |
| TV-PG  |    861 |
| R      |    799 |
| PG-13  |    490 |

**[INSERT IMAGE HERE — `TASK5_Audience_Rating_Insights_Dashboard.png`]**

The dashboard uses PivotTables and visualizations to compare rating distribution across Movies and TV Shows.

---

# 📊 Task 6 — Executive Analytics Dashboard

The final dashboard consolidates the major findings into an executive-level view.

### Key Performance Indicators

| KPI                |         Value |
| ------------------ | ------------: |
| Total Titles       |         8,790 |
| Movies             |         6,126 |
| TV Shows           |         2,664 |
| Most Common Rating | TV-MA — 3,205 |

The dashboard brings together:

* Content type distribution
* Release trends
* Content categories
* Rating information
* Interactive filters

**[INSERT IMAGE HERE — `TASK6_Executive_Netflix_Analytics_Dashboard.png`]**

---

# 📈 Key Insights

### 01 — Movies represent the majority of the catalog

Movies account for **6,126 titles**, approximately **69.7%** of the dataset.

TV Shows account for approximately **30.3%**.

### 02 — United States has the largest country representation

The United States appears with **3,240 titles** in the country field.

### 03 — TV-MA is the most common rating

TV-MA appears on **3,205 titles**, making it the most frequently occurring rating.

### 04 — 2018 records the highest displayed release-year total

The release-year analysis shows **1,146 titles in 2018**.

### 05 — Movie and TV Show patterns change over time

Movies generally have higher yearly counts, but TV Shows exceed Movies in the displayed **2021** data.

---

# 🛠️ Tools & Skills

### Tools

* **Microsoft Excel**
* **Power Query**
* **PivotTables**
* **PivotCharts**
* **Slicers**
* **Data Visualization**

### Skills Demonstrated

* Data cleaning
* Data validation
* Data profiling
* Exploratory data analysis
* PivotTable analysis
* Dashboard development
* KPI creation
* Data visualization
* Insight generation
* Business-oriented reporting

---

# 🔄 Analytical Workflow

```text
Raw Dataset
     ↓
Power Query Import
     ↓
Data Profiling
     ↓
Data Cleaning
     ↓
Data Validation
     ↓
PivotTables
     ↓
PivotCharts
     ↓
Interactive Dashboards
     ↓
Insights
```

**[INSERT IMAGE HERE — `load_data.png` showing the dataset being loaded into Power Query]**

---

# ⚠️ Project Limitations

The dataset contains **content metadata**, not actual Netflix business-performance data.

Therefore, this project does not attempt to measure:

* Revenue
* Profit
* Subscribers
* Watch time
* Customer churn
* Viewer engagement
* Content ROI

The findings are therefore focused on **catalog structure, distribution, and metadata patterns**.

---

# 🚀 Future Improvements

With additional business data, the analysis could be expanded into:

### Content Performance

* Views
* Watch time
* Completion rate
* Viewer ratings
* Engagement

### Customer Analytics

* Subscriber behavior
* Churn
* Retention
* Viewing preferences

### Advanced Analytics

* SQL-based analysis
* Python/Pandas
* Power BI
* Statistical analysis
* Predictive modeling

---

# 📸 Project Screenshots

## Data Cleaning & Chart Preparation

**[INSERT `TASK1_Data_Cleaning_&_Chart_Preparation.png` HERE]**

## Country-Wise Analysis

**[INSERT `TASK3_Country-Wise_Content_Analysis_Dashboard.png` HERE]**

## Release Trend Analysis

**[INSERT `TASK4_Netflix_Release_Trend_Visualization.png` HERE]**

## Audience Rating Analysis

**[INSERT `TASK5_Audience_Rating_Insights_Dashboard.png` HERE]**

## Executive Dashboard

**[INSERT `TASK6_Executive_Netflix_Analytics_Dashboard.png` HERE]**

---

# 🎓 Internship Context

This project was completed as part of the **Auspify Technologies Internship Program**, providing practical experience in applying Excel-based data analytics to a structured content dataset.

The project covered the full analytical process from **data preparation and validation to visualization, dashboard development, and insight generation**.

---

# 👨🏽‍💻 Author

### Alade Zaccheous Kehinde

**Data Analyst | Python Developer | Django Developer**

**GitHub:** `ZacchTech`
**LinkedIn:** `ZacchTech`

---

## 🏁 Final Takeaway

This project demonstrates the ability to move beyond simply creating charts in Excel and follow a structured analytics workflow:

> **Understand the data → Clean it → Validate it → Analyze it → Visualize it → Communicate the findings**

The final solution transforms a raw content catalog into an interactive Excel-based analytical report covering **content composition, countries, release trends, ratings, categories, and executive-level insights**.

---

### 📌 Images I recommend you actually place

| README section | Image to insert                                     |
| -------------- | --------------------------------------------------- |
| Header         | Auspify logo                                        |
| Data Cleaning  | `type_in_power_Query.png`                           |
| Task 1         | `TASK1_Data_Cleaning_&_Chart_Preparation.png`       |
| Task 3         | `TASK3_Country-Wise_Content_Analysis_Dashboard.png` |
| Task 4         | `TASK4_Netflix_Release_Trend_Visualization.png`     |
| Task 5         | `TASK5_Audience_Rating_Insights_Dashboard.png`      |
| Task 6         | `TASK6_Executive_Netflix_Analytics_Dashboard.png`   |
| Workflow       | `load_data.png`                                     |

**One important thing:** when you send the **actual dataset**, I want to do one final verification pass over the README numbers and insights. That way, the README will be based on the actual final dataset rather than only the screenshots, and we can confidently call it the **final GitHub version**.
