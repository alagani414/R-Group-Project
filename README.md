<div align="center">
    <h1 align="center">Beyond the Net: Insights into Volleyball Performance at Paris 2024</h1>
    <p align="center">An analytical deep dive into Olympic volleyball performance metrics.</p>
</div>

---

## Project Overview
This project analyzes **volleyball and beach volleyball performance** at the 2024 Paris Olympics, combining athlete attributes (height, age, gender) with team dynamics and match outcomes. Key goals include:
- Identifying correlations between physical traits (e.g., height) and success 🏆
- Visualizing regional participation and dominance 🌍
- Comparing performance trends between indoor volleyball and beach volleyball 🏖️

---

## Data Sources
- **Primary Datasets**: [Kaggle](https://www.kaggle.com/datasets/piterfm/paris-2024-olympic-summer-games)
  `teams.csv`, `athletes.csv`, `Volleyball.csv`, `Beach Volleyball.csv`

---

## Data Adjustments
### Key Steps:
1. **Column Selection & Renaming**  
   Focused on participant details, event results, and athlete attributes.
2. **Merging Datasets**  
   Combined team rosters with athlete profiles and match outcomes.
3. **Derived Metrics**  
   Calculated `win_percentage` and handled missing values.
4. **Geospatial Enrichment**  
   Linked countries to geographic coordinates for mapping.

---

## Analysis & Visualizations
### 1. Geospatial and Statistical Dashboard
- **Scatterplot**: Total matches vs. win percentage (experience correlates with success).  
- **Bar Chart**: Match participation by country (USA leads in total matches).  
- **World Map**: Highlights regional dominance (Americas/Europe vs. underrepresented Africa).

### 2. Parallel Coordinate Plots
- Compared standardized metrics (age, height, wins) across countries.  
- **Key Insight**: Tight age clustering (most athletes are 25-30 yrs), broader win variability.

### 3. Athlete Height Analysis
- **Scatter Plot**: Height distribution by gender.  
- **Country Trends**: Taller nations (Cuba: 202.5 cm avg) don’t always win more, indicating height isn’t the sole factor.

---

## Tools & Libraries
```r
# R Packages
library(ggplot2)    # Visualization
library(ggiraph)    # Interactive plots
library(tidyverse)  # Data wrangling and cleaning