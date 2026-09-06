# GEMA Education — Competition Registrations Analysis

**Data Analytics Internship — Practical Assignment**
Prepared by: **Ankita Daweshar**

## Objective

GEMA Education runs multiple student competitions throughout the year. This project analyzes how 2026 competition registrations compare to the same period in 2025 (Jan 1 – Sep 4, both years), to help management understand current performance and spot trends worth acting on.

## Headline Result

**Overall registrations are up 19.4% year-over-year** (1,800 → 2,150), with every one of the 8 competitions growing — none declined. Growth ranges from +10.0% (AI & Robotics Challenge) to +32.9% (Student Speaker Competition). Full findings are in the summary report (see below).

## Folder Structure
```
GEMA_Registrations_Project/
│
├── raw dataset/
│ ├── GEMA_Competition_Registrations_2025.xlsx
│ └── GEMA_Competition_Registrations_2026.xlsx
│ → Original, untouched source files as provided.
│
├── clean dataset/
│ ├── clean_2025.csv
│ ├── clean_2026.csv
│ └── GEMA_Cleaned_Registrations.xlsx
│ → Cleaned registration data (duplicates removed, dates standardized,
│ competition/school names normalized, missing values handled).
│ See the "Cleaning Log" tab inside the .xlsx for full details.
│
├── analysis and summary/
│ ├── GEMA_Registration_Analysis.ipynb (Python notebook — full workflow)
│ ├── GEMA_Analysis_Workbook.xlsx (Excel version — formula-driven tables & charts)
│ ├── GEMA_Findings_Summary.docx
│ ├── GEMA_Findings_Summary.pdf
│ └── output images/
│ ├── chart_competition_comparison.png
│ ├── chart_monthly_trend.png
│ └── chart_weekly_trend.png
│ → Cleaning → analysis → trend detection, in both notebook and Excel form.
│ The findings summary is the short written report for management,
│ with dashboard screenshots and recommendations included.
│
└── Dashboard/
└── GEMA_Dashboard.pbix
→ 3-page Power BI dashboard (Overview, Competition Analysis, Trend Analysis).
Open in Power BI Desktop to interact with it; screenshots of every page
are also included in the findings summary PDF for quick viewing.
```

## How to Reproduce This Analysis

1. Open `analysis and summary/GEMA_Registration_Analysis.ipynb` in Jupyter, VS Code, or Google Colab.
2. Run all cells — it reads the raw files, cleans them, and produces every table and chart used in this project.
3. To rebuild the Power BI dashboard: import `clean dataset/GEMA_Cleaned_Registrations.xlsx` into Power BI Desktop, append the two year-sheets into one `Registrations` table, and build measures/visuals as documented in the analysis workbook.

## Key Findings (see full summary for details)

- Total registrations: **1,800 → 2,150 (+19.4%)** over the identical Jan 1–Sep 4 window.
- **Fastest growing:** Student Speaker Competition (+32.9%), International Coding Olympiad (+26.1%), International Science Olympiad (+25.1%).
- **Slowest growing:** AI & Robotics Challenge (+10.0%), Winter Painting Competition (+11.6%), International Mathematics Olympiad (+14.9%).
- **Momentum shift:** Young Innovators Challenge nearly doubled in the last 4 weeks alone (+125%), despite modest full-period growth — worth a promotional push now.
- International Science and School Olympiads are cooling off in recent weeks despite strong overall numbers.

Full recommendations are in `analysis and summary/GEMA_Findings_Summary.pdf`.

## Data Note

Both source files cover the same calendar window (Jan 1 – Sep 4) in their respective years, so no additional date-range filtering was needed for a fair year-over-year comparison. September figures reflect a partial month in both years, not a decline.
