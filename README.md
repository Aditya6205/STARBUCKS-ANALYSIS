# Starbucks Global Footprint & Menu Macro-Nutrient Optimization Dashboard

## 📌 Project Overview
This repository contains a comprehensive, business-driven business intelligence project utilizing **Power BI Desktop** to analyze Starbucks' global store configurations alongside itemized beverage nutritional profiles. 

Rather than simply displaying raw data, this project addresses real-world corporate challenges: **navigating shifting global health trends**, **evaluating market saturation limits**, and **identifying high-margin product opportunities** within the functional beverage market.

### 🖼️ Executive Dashboard Preview
> *Refer to the file named verbatim `Screenshot (91).jpg` in the root directory to view the complete interactive layout.*

---

## 🚀 Key Business Problems Addressed & Data Insights

### 1. Navigating the Global "Healthy Beverage" Shift
*   **The Problem:** Shifting consumer behavior is driving demand away from high-calorie, sugar-heavy items. Starbucks needs menu optimization models to protect volume sales without sacrificing product quality.
*   **The Insights:** 
    *   The baseline menu averages **193.87 calories** and **32.96g of sugar** per beverage.
    *   `Frappuccino® Blended Coffee` stands out as the highest sugar offender, averaging a staggering **57.08g of sugar** per drink.
    *   **The Milk Lever:** Transitioning standard drink formulations from `Whole Milk` to `2% Milk` slashes average drink calories from **283.75** down to **218.00** while maximizing average protein extraction to its highest menu baseline of **9.62g**.
*   **Strategic Action:** Recommend that product development teams standardize **2% Milk** as the default menu baseline for blended options, reducing total sugar exposure by **44.3%** while capturing the macro-conscious fitness demographic.

### 2. Retail Expansion & Asset Ownership Mix Strategy
*   **The Problem:** Mitigating capital expenditure risk in international territories while determining market penetration boundaries to avoid internal brand cannibalization.
*   **The Insights:** 
    *   The complete global footprint spans **25,600 stores** across **73 distinct countries**.
    *   The geographic distribution is heavily top-weighted: the **United States** leads with **13,608 stores (53.1%)**, followed by **China** with **2,734 stores (10.6%)**, and **Canada** with **1,468 stores (5.7%)**.
    *   **Operational Blueprint:** **46.6%** of locations operate via high-control `Company Owned` structures, while **36.6%** utilize a low-overhead `Licensed` model, and **15.5%** use `Joint Ventures`.
*   **Strategic Action:** With the North American market entering high saturation limits ($>53\%$ footprint), future international growth capital should shift away from resource-intensive Company-Owned structures and aggressively pivot toward the **Licensed model (36.6%)** to scale presence across emerging regions at low capital risk.

### 3. Maximizing the Functional Beverage Market Segment
*   **The Problem:** Capitalizing on the high-margin functional energy beverage boom by identifying which core products deliver the highest concentration of caffeine with minimal calorie payloads.
*   **The Insights:** 
    *   A massive functional disparity exists between traditional coffee blends and dessert-oriented treats. 
    *   A standard `Venti Brewed Coffee` leads menu efficiency, outputting **410mg of caffeine** for only **5 calories**, resulting in a calculated **Caffeine Efficiency Index of 82.00**.
    *   Conversely, specialty sweet drinks routinely collapse beneath an index threshold of **1.00**, costing hundreds of calories for a minimal energy return.
*   **Strategic Action:** Implement a highly targeted, data-backed B2B marketing framework (*"Maximum Focus, Zero Crash"*) bundling products maintaining a Caffeine Efficiency Index $> 50$. This secures high-retention customer loyalty among white-collar corporate professionals looking for healthy mid-day energy boosts.

---

## 🛠️ Technical Implementation & Data Engineering

*   **Data Sources:** Analyzed raw structural business datasets including `directory.csv` (store logistics) and `starbucks.csv` (menu nutrition metrics).
*   **ETL & Data Cleaning (Power Query):**
    *   Cleaned structural text columns, handled missing values, and trimmed trailing whitespace anomalies.
    *   Parsed irregular string values inside the `Caffeine (mg)` column (e.g., converting text occurrences like *"Varies"* to numeric baselines) to prevent calculation errors.
    *   Generated localized conditional grouping arrays to aggregate irregular milk variations (`Short Nonfat Milk`, `Soymilk`, `2% Milk`) into clean, parent categorical dimensions.
*   **Data Modeling & Advanced DAX:**
    *   Constructed relational linkages connecting retail operations metrics with localized product offerings.
    *   Engineered custom statistical measures including the **Caffeine Efficiency Index**:
      $$\text{Caffeine Efficiency Index} = \frac{\text{Clean Caffeine (mg)}}{\text{Average Calories}}$$
*   **UI/UX Dashboard Styling:**
    *   Implemented a bespoke design incorporating Starbucks' corporate brand identity palette (signature forest greens, soft creams, minimalist modern containers).
    *   Structured intuitive KPI metric blocks, line charts mapping caloric degradation trends, and high-resolution graphical card layouts to highlight top-performing products.

---

## 📈 Impact Summary (STAR Method)
*   **Situation:** Analyzed international operational retail footprints alongside complex product recipe matrices to solve market saturation challenges and address changing nutritional trends.
*   **Task:** Engineered a robust business intelligence infrastructure converting **25,600 operational store profiles** and extensive ingredient records into data stories tailored for C-suite decision-makers.
*   **Action:** Developed automated ETL pipelines in Power Query, resolved column data type mismatches, mapped multi-tiered global distribution data, and built diagnostic index equations utilizing custom DAX structures.
*   **Result:** Modeled explicit menu optimization scenarios capable of reducing retail sugar exposure across core portfolios by **44.3%**, and delivered high-impact growth frameworks optimizing real estate ownership distributions across **73 countries**.

---

## 📂 Repository Contents
*   `STARBUCKS_ANALYSIS.pbix` - The primary Power BI data model and dashboard file.
*   `starbucks.csv` - Raw menu nutritional dataset containing ingredient profiles, calorie weights, and macro listings.
*   `directory.csv` - Complete spatial real estate tracking data covering global store IDs, long/lat mappings, and ownership structures.
*   `Screenshot (91).jpg` - High-definition visual screen capture showcasing the active dashboard interface.

---
### 🛠️ Tools Used
*   **Power BI Desktop** (Data Modeling, DAX, Report Design)
*   **Power Query** (M Language - ETL, Data Parsing & Formatting)
*   **Excel** (Initial Data Inspection)
