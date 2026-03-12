# Anthrax in Europe: A One Health Perspective

**Authors:** Vikaat Ravi & Samarth Gupta  
**Course:** INFO 201 — University of Washington

---

## Project Overview

This project analyzes the distribution of anthrax across Europe using a **One Health** framework — an approach that recognizes the interconnection between human health, animal health, and the environment. By combining human disease surveillance data with animal outbreak data, we explore geographic patterns and potential links between animal outbreaks and human anthrax cases.

---

## Research Questions

1. **What is the proportion of human anthrax cases among the most affected European countries?**
2. **Which European countries report the highest number of animal anthrax outbreaks?**
3. **How does the intensity of animal outbreaks vary across different countries and years?**

---

## Data Sources

| Source | Description | Link |
|--------|-------------|------|
| **ECDC** | European Centre for Disease Prevention and Control — confirmed human anthrax cases across European countries | [ECDC Surveillance Atlas](https://atlas.ecdc.europa.eu/public/index.aspx?Instance=GeneralAtlas) |
| **WOAH** | World Organisation for Animal Health — reported animal anthrax outbreaks submitted via the WAHIS system | [WAHIS Event Management](https://wahis.woah.org/#/event-management) |

---

## Dashboard Features

- **Interactive visualizations** built with `plotly` and `ggplotly`
- **Pie chart** showing the proportional share of human cases among the top 5 most affected countries
- **Bar chart** comparing cumulative animal anthrax outbreaks by country
- **Heat map** visualizing outbreak intensity across countries and years (2007–present)

---

## Files

| File | Description |
|------|-------------|
| `anthrax_dashboard.qmd` | Quarto source file for the dashboard |
| `anthrax_dashboard.html` | Rendered interactive HTML dashboard |
| `ecdc_data.csv` | Human anthrax case data from ECDC |
| `woah_data.csv` | Animal anthrax outbreak data from WOAH |

---

## How to Run Locally

1. Clone this repository
2. Open `anthrax_dashboard.qmd` in RStudio
3. Ensure the following R packages are installed:
```r
install.packages(c("tidyverse", "ggplot2", "lubridate", "plotly"))
```
4. Place `ecdc_data.csv` and `woah_data.csv` in the same directory as the `.qmd` file
5. Click **Render** in RStudio to generate the dashboard

---

## Limitations

- Surveillance quality varies across countries — reported zeros may reflect underreporting rather than true absence of disease
- Only country-level aggregates are used to protect individual privacy
- Additional data (e.g., livestock populations, vaccination coverage, environmental risk factors) could improve future analyses

---

## Contact

| Name | Email |
|------|-------|
| Vikaat Ravi | sravi03@uw.edu |
| Samarth Gupta | sammyy18@uw.edu |
