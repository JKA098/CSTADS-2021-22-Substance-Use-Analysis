# CSTADS 2021–22 Substance Use Analysis 📊🗺️

![License](https://img.shields.io/badge/license-OGL--Canada-blue)
![R](https://img.shields.io/badge/made%20with-R-276DC3)
![Data](https://img.shields.io/badge/data-Health%20Canada-important)
![Survey](https://img.shields.io/badge/CSTADS-2021--22-green)
![Geospatial](https://img.shields.io/badge/mapping-leaflet-lightgrey)
![Big Data](https://img.shields.io/badge/big%20data-enabled-orange)


---

## 📌 Project Summary

The **Canadian Student Tobacco, Alcohol and Drugs Survey (CSTADS)** 2021–22 dataset is analyzed to explore:

* Provincial variation in youth **cannabis**, **alcohol**, and **tobacco** use
* The impact of **cannabis legalization**
* Access networks for each substance
* Regional policy implications using **geospatial** and **network** analysis

**Dataset Source:** [Government of Canada Open Data Portal](https://open.canada.ca/data/dataset/1f15ca45-8bfd-4f9c-9ec6-2c0c440e69c2)

**Survey Years:** Sept 2021 – June 2022
**Target Group:** Grades 7–12 (Secondary I–V in Quebec) students across 9 Canadian provinces

---

## 🔧 Setup & Tools

This project was built in **RStudio** using the following packages:

```r
library(tidyverse)
library(sf)
library(leaflet)
library(igraph)
library(ggnetwork)
library(ggplot2)
library(webshot2)
```

---

## 🌍 Geospatial & Network Analysis

We performed:

* Binary transformation of substance use variables
* Merging shapefiles with survey data
* **Interactive maps (leaflet)**
* **Bar plots** by province
* **Network graphs** showing access routes

### 🗺️ Map Outputs

* Cannabis use by province ![Cannabis](picture_to_use/canabis_use_1.png)
* Smoking use by province ![Smoking](picture_to_use/smoking_use_1.png)
* Alcohol use by province ![Alcohol](picture_to_use/alcohol_use_1.png)

### 🔗 Access Networks

* Cannabis, Alcohol, and Cigarette access channels were visualized using `igraph + ggnetwork`

---

## 📁 Folder Structure

```plaintext
📁 cstads_substance_analysis/
├── 📊 plots/                # bar charts per province
├── 🌍 maps/                # leaflet visualizations
├── 📄 cleaned_dataset.csv   # cleaned input file
├── 📂 picture_to_use/       # embedded images (e.g., canabis_use_1.png)
├── 📓 analysis.qmd          # Quarto document (Geospatial & Network)
└── README.md
```

---

## 📋 License & Citation

This project uses data governed by the **Open Government License – Canada**.

📌 **Required Acknowledgment**:

> Data used were obtained from Health Canada’s CSTADS 2021–22 PUMF. Health Canada has not reviewed, approved, or endorsed this analysis.

📚 **Cite As**:

* Health Canada. Canadian Student Tobacco, Alcohol and Drugs Survey (CSTADS) 2021–22 Public Use Microdata File \[Data file]. Government of Canada: Ottawa (ON); 2023.

📩 **Contact:**  [ODRS-BRSD@hc-sc.gc.ca](mailto:ODRS-BRSD@hc-sc.gc.ca)

---


*For extended documentation and discussion, refer to the `.qmd` source file or rendered PDF.*
