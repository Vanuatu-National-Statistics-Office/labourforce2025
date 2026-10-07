# Vanuatu Labour Force Survey 2025 – Interactive Dashboard

An interactive dashboard of the key results of the **Vanuatu Labour Force Survey (LFS) 2025**, published by the **Vanuatu Bureau of Statistics (VBoS)**.

The dashboard presents the 29 LFS 2025 output tables (T5.1–T30) as charts and tables. It covers population, labour force participation, employment, labour underutilisation, informality, hours and earnings, own-use production, and migration and labour mobility.

🔗 **View the dashboard:** `https://<your-github-username>.github.io/<repository-name>/`

---

## Features

- **Overview page** with headline indicators: population, employment, labour force participation, unemployment, youth NEET (not in employment, education or training), informal employment and household emigration
- **Sidebar navigation** with a page for every table, grouped by topic, plus a search box
- **Interactive charts** comparing results by sex (male / female) or by area (urban / rural), with hover tooltips
- **The full published table** on every table page, with a **Download CSV** button
- **Light and dark themes**, and a layout that works on desktop, tablet and mobile
- **VBoS colours**, taken from the Bureau's logo and checked for colour-blind readability
- **A single self-contained file** (`index.html`): it needs no internet connection, installation or server software to view

---

## Tables included

| Topic | Tables |
|---|---|
| **Population** | T5.1 Population by age & sex · T5.2a Educational attainment · T5.2b Population by region · T6.1 Working-age population · T6.2 Working-age by region |
| **Labour force** | T7 Labour force status · T8 Labour force participation rate · T9 Employment-to-population ratio |
| **Employment** | T10 Employment by sector · T11 Status in employment (ICSE-18) · T12 ICSE-18-A categories · T13 Detailed ICSE-18-A status · T14 Economic risk (ICSE-18-R) · T15 Risk & authority · T16 Occupation (ISCO) |
| **Labour underutilisation** | T17 Labour underutilisation (LU1–LU4) · T18 Persons outside the labour force · T19 Youth NEET rate · T20 NEET: 13th vs 19th ICLS |
| **Informality** | T21 Informal employment · T22 Employment in the informal sector |
| **Hours & earnings** | T23 Hours worked · T24 Monthly wage · T25 Wage by age group |
| **Own-use production** | T26 Subsistence & own-use producers · T27 Own-use producers of foodstuffs |
| **Migration & mobility** | T28 Household emigration rate · T29 Household members abroad · T30 Labour mobility programmes |

---

## Concepts and definitions

- Labour statistics follow the **19th International Conference of Labour Statisticians (ICLS)** standards unless stated otherwise.
- Under the 19th ICLS definition, persons producing goods mainly for their own household's use (subsistence) are **not counted as employed**. As a result, the 19th ICLS definition counts more youth as NEET than the earlier 13th ICLS definition. Table T20 compares the two.
- Industry follows **ISIC Rev. 4**, occupation follows **ISCO-08**, and status in employment follows **ICSE-18**.
- Indicators refer to persons aged **15 and over** unless noted otherwise. Educational attainment refers to persons aged 16 and over.

---

## Notes on presentation

- **Age groups (T5.1):** the age group labelled "55–60" in the source table is shown as **55–59**, as agreed by the publication review team.
- **Employment by sector (T10):** in the charts, *Wholesale and retail trade; repair of motor vehicles* is shown as its three published sub-categories: retail trade, wholesale trade, and motor vehicle trade & repair. *Accommodation and food service activities* is shown as accommodation activities and food service activities. The full table keeps the published sector totals.
- **Short chart labels:** some long category names are shortened on charts, for example "Wholesale trade" stands for "Wholesale trade excluding motor vehicles or Other wholesale trade". The full published wording appears in each table.
- **Rounding:** sub-categories may not add up exactly to their totals because of rounding in the source tables.

---

## Repository contents

| File | Purpose |
|---|---|
| `index.html` | The dashboard. Open it in any web browser. |
| `README.md` | This file. |

---

## Updating the dashboard

The dashboard's data is generated from the LFS Excel tables by the `build_data.py` script, which is kept with the source tables.

1. Update the Excel tables (`T5.1_…xlsx` to `T30_…xlsx`).
2. Run the script, which needs Python 3 and the `openpyxl` package:
   ```bash
   pip install openpyxl
   python build_data.py
   ```
3. Upload the new `index.html` to this repository, replacing the old one. The website refreshes within a few minutes.

---

## Source and citation

**Source:** Vanuatu Bureau of Statistics, *Vanuatu Labour Force Survey 2025*.

Suggested citation:
> Vanuatu Bureau of Statistics (2026). *Vanuatu Labour Force Survey 2025 – Interactive Dashboard*. Port Vila: Vanuatu Bureau of Statistics.

---

## Contact

**Vanuatu Bureau of Statistics**
Bureau des Statistiques du Vanuatu

For questions about the data or this dashboard, please contact VBoS: <!-- stats@vanuatu.gov.vu / vbos.gov.vu /+678 9022110  -->

