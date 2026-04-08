# Open Data for African Data-Driven Growth Newsletter

A curated, open-access data repository backing the research and data visualizations published in the **African Data-Driven Growth Newsletter** — a publication focused on sharing insights toward data-driven business growth in African markets.

> *"While technology scales systems, storytelling scales truth."*

---

## 🎯 Purpose

This repository hosts the raw and processed datasets used to:

- Back up research published in the newsletter
- Power data visualizations on African business and economic trends
- Provide transparent, reproducible analysis starting from Uganda and expanding across East Africa

All data is sourced from credible, publicly available sources and is made freely available here for journalists, researchers, business analysts, and curious minds.

---

## 🗂️ Repository Structure

```
data/
├── uganda/              # Uganda-specific datasets
│   ├── economy/         # GDP, inflation, trade, fiscal data
│   ├── demographics/    # Population, urbanization, household surveys
│   ├── technology/      # Internet, mobile, fintech adoption
│   └── business/        # Company registrations, sectors, investment
├── east-africa/         # Regional datasets covering EAC member states
│   ├── economy/
│   ├── demographics/
│   └── technology/
└── africa-wide/         # Pan-African datasets
    ├── economy/
    └── technology/

visualizations/          # Chart configs, notebooks, and visual assets
```

---

## 📊 Available Datasets

See the full **[Data Catalog](DATA_CATALOG.md)** for a browsable index of all datasets, including descriptions, sources, and coverage periods.

---

## 🌍 Geographic Focus

| Priority | Region |
|----------|--------|
| 1 | Uganda |
| 2 | East Africa (Kenya, Tanzania, Rwanda, Burundi, South Sudan, DRC) |
| 3 | Africa-wide |

---

## 📁 Data Format Standards

- **File format:** CSV (UTF-8 encoded) for tabular data; GeoJSON for geographic data
- **Date format:** ISO 8601 (`YYYY` for annual, `YYYY-MM` for monthly, `YYYY-MM-DD` for daily)
- **Numeric values:** Plain numbers without currency symbols or commas; units specified in column headers or a companion `README.md`
- **Missing values:** Left blank (empty cell) — not `N/A`, `null`, or `0`
- **Column names:** `snake_case`, English

---

## 🔗 Primary Data Sources

| Source | Description | URL |
|--------|-------------|-----|
| World Bank Open Data | GDP, development indicators, trade | https://data.worldbank.org |
| Uganda Bureau of Statistics (UBOS) | National statistics for Uganda | https://www.ubos.org |
| African Development Bank (AfDB) | African economic and social data | https://dataportal.opendataforafrica.org |
| GSMA Intelligence | Mobile connectivity data | https://www.gsma.com/intelligence |
| ITU (International Telecommunication Union) | ICT indicators | https://www.itu.int/en/ITU-D/Statistics |
| Knomad / World Bank | Remittances and migration | https://www.knomad.org |
| UN Comtrade | International trade statistics | https://comtradeplus.un.org |
| Uganda Investment Authority (UIA) | Investment and business data | https://www.ugandainvest.go.ug |

---

## 🤝 Contributing

Want to add a dataset or improve an existing one? Please read the **[Contributing Guide](CONTRIBUTING.md)** first.

---

## 📜 License

All datasets in this repository are shared under the **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)** license unless a dataset's own license (noted in the Data Catalog) is more restrictive.

You are free to share and adapt the data for any purpose, as long as you give appropriate credit.

---

## ✉️ Newsletter

Follow the newsletter for the stories behind this data:
[African Data-Driven Growth Newsletter](https://github.com/ronnielutaro/Open-Data-for-African-Data-Driven-Growth-Newsletter)
