# Formula 1 Relational Data Engineering (13-Table Schema)

## Project Overview

This repository contains a **comprehensive relational database ecosystem** built from historical **Formula 1 (F1) data**. The project focuses on architecting a **13-table relational schema** that enables deep-dive analytics across **over 70 years of racing history**, ranging from millisecond-level telemetry to season-long driver and constructor standings.

The work emphasizes **data modeling, referential integrity, and scalable analytical design** within a complex, real-world dataset.

---

## Key Data Engineering Workflows

### 🧩 Relational Schema Architecture
- Designed and implemented a schema integrating **13 interconnected tables**
- Established complex **Primary Key (PK)** and **Foreign Key (FK)** relationships using:
  - `raceId`
  - `driverId`
  - `constructorId`
- Enabled efficient multi-table joins across race context, telemetry, and outcomes

### ⏱️ Granular Telemetry Processing
- Managed high-frequency telemetry datasets, including:
  - `lap_times_mod.csv`
  - `pit_stops_mod.csv`
- Enabled analysis at **lap-level and pit-stop-level granularity**
- Supported performance benchmarking and race strategy analysis

### ✅ Data Integrity & Consistency
- Leveraged the provided **Data Dictionary** to enforce:
  - Consistent data types
  - Standardized units (e.g. milliseconds for all timing data)
- Maintained referential integrity across all 13 tables

### 🔗 Feature Integration
- Integrated session-level data from `qualifying_mod.csv` with final outcomes in `results_mod.csv`
- Enabled analysis of:
  - Grid position vs. finishing position
  - Qualifying performance impact on race results

---

## Data Dictionary & Dataset Ecosystem

This project utilizes a **robust metadata library** that documents every field across the 13-table schema.

### Dataset Categories and Files

**Core Entities**  
- `drivers_mod.csv`  
- `constructors_mod.csv`  

**Race Context**  
- `races_mod.csv`  
- `circuits_mod.csv`  

**Telemetry**  
- `lap_times_mod.csv`  
- `pit_stops_mod.csv`  
- `qualifying_mod.csv`  

**Outcomes**  
- `results_mod.csv`  
- `status_mod.csv`  

**Standings**  
- `driver_standings_mod.csv`  
- `constructor_standings_mod.csv`  
- `constructor_results_mod.csv`  

---

## Technical Stack

- **Language:** Python (Pandas, NumPy)  
- **Metadata Management:** `f1db_data_dictionary.txt` for schema documentation  
- **Analysis Focus:**  
  - Time-series analysis  
  - Relational data engineering  
  - Performance metrics and trend analysis  

---

## Academic Context

- **Module:** Data Wrangling (DW)  
- **Objective:**  
  To demonstrate mastery in handling **high-dimensional relational datasets**, enforcing **referential integrity**, and performing structured analytics within a complex data ecosystem.
