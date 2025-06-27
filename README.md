# City of Angels Crime Analysis 😎

Welcome to the Los Angeles crime‐analysis project! In this repo we dive into the City of Angels—Tinseltown’s warm beaches, palm-tree boulevards and glitzy studios—then turn our attention to the complex reality of crime in America’s entertainment capital. You’ll find code, notebooks, and guidance for exploring LA’s crime dataset, uncovering patterns, and empowering the LAPD to allocate resources where they matter most.

---

## Table of Contents

1. [Project Overview](#project-overview)  
2. [Dataset Description](#dataset-description)  
3. [Column Glossary](#column-glossary)  
4. [Environment & Dependencies](#environment--dependencies)  
---

## Project Overview

Los Angeles is known for its sunshine and silver screens, but high population density brings challenges in public safety. This project supports the LAPD by:

- Profiling crime trends by geography, time, and victim demographics  
- Identifying hotspots and high‐risk windows  
- Equipping decision‐makers with actionable insights  

Our single data source is a modified snapshot from Los Angeles Open Data, containing every reported crime with location, type, victim details, and status.

---

## Dataset Description

**File**: `crimes.csv`  
A cleaned, anonymized extract of LA crime records. Each row represents one reported incident.

---

## Column Glossary

| Column         | Description                                                                                                      |
|----------------|------------------------------------------------------------------------------------------------------------------|
| **DR_NO**      | Division of Records Number (2-digit year + area ID + 5-digit file).                                              |
| **Date Rptd**  | Date reported (MM/DD/YYYY).                                                                                      |
| **DATE OCC**   | Date of occurrence (MM/DD/YYYY).                                                                                 |
| **TIME OCC**   | Time of occurrence in 24-hour format (e.g., 0830 for 8:30 AM).                                                    |
| **AREA NAME**  | Patrol division name (e.g., “77th Street Division”).                                                             |
| **Crm Cd Desc**| Crime description (type of offense committed).                                                                   |
| **Vict Age**   | Victim’s age in years.                                                                                           |
| **Vict Sex**   | Victim’s sex: F=Female, M=Male, X=Unknown.                                                                       |
| **Vict Descent**| Victim’s descent/ethnicity (e.g., H=Hispanic, W=White, B=Black, etc.).                                         |
| **Weapon Desc**| Weapon used, if any (e.g., “Handgun”, “Knife”, “None”).                                                          |
| **Status Desc**| Status of the crime case (e.g., “Open”, “Arrest”, “Exceptional Cleared”).                                        |
| **LOCATION**   | Street‐level address or intersection where the crime took place.                                                 |

---

## Environment & Dependencies

- Python 3.8+  
- pandas  
- numpy  
- matplotlib / seaborn  
- geopandas / folium (for mapping)  
- scikit-learn (for clustering or predictive models)  
- jupyterlab  

Install with:
```bash
pip install pandas numpy matplotlib seaborn geopandas folium scikit-learn jupyterlab
```

---

