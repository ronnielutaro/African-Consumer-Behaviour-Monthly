# Contributing to the Open Data Repository

Thank you for your interest in contributing! This repository welcomes open datasets that support research and data-driven storytelling about business growth in African markets — starting with Uganda and East Africa.

---

## Ways to Contribute

1. **Add a new dataset** — CSV files with clean, well-documented data
2. **Update an existing dataset** — extend coverage years or fix errors
3. **Improve documentation** — better READMEs, source notes, or the Data Catalog
4. **Report a data issue** — open a GitHub Issue if you spot incorrect data or a broken source link

---

## Before Adding a Dataset

Please check:

- [ ] The dataset is **not already included** (check [DATA_CATALOG.md](DATA_CATALOG.md))
- [ ] The data is from a **credible, publicly available source** (government statistics, World Bank, UN agencies, peer-reviewed surveys, etc.)
- [ ] The source permits redistribution (open license — CC BY, public domain, or similar)
- [ ] The data is **relevant** to African markets, business, economy, technology, or demographics

---

## Dataset Requirements

### File format
- Use **CSV (UTF-8)** for tabular data
- Use **GeoJSON** for geographic/spatial data
- Keep one dataset per file; do not combine unrelated indicators in one file

### Naming convention
- Use `snake_case` file names, all lowercase, no spaces
- Be descriptive: `internet_penetration_annual.csv` not `data1.csv`
- Include `_annual`, `_monthly`, or `_quarterly` in the name to indicate frequency

### Column standards
| Rule | Example |
|------|---------|
| `snake_case` column names | `gdp_usd`, `year`, `country_name` |
| ISO 8601 date/year columns | `year` = `2023`; `date` = `2023-06` |
| Numeric values only (no symbols) | `45600000000` not `$45.6B` |
| Units in column header or README | `gdp_current_usd_billions` |
| Empty cell for missing values | not `N/A`, `null`, or `0` |
| Country names in English | `Uganda` not `UGA` (ISO code can be a separate column) |
| Include ISO 3166-1 alpha-3 country codes | `country_code` column |

### Companion README
Each dataset file should have a `README.md` in its directory (one per topic folder, not per file) that notes:
- What the data represents
- The unit of measurement
- The data source and URL
- The date the data was last updated
- Any known caveats or gaps

---

## Folder Placement

Place datasets in the most specific applicable folder:

```
data/
├── uganda/
│   ├── economy/
│   ├── demographics/
│   ├── technology/
│   └── business/
├── east-africa/
│   ├── economy/
│   ├── demographics/
│   └── technology/
└── africa-wide/
    ├── economy/
    └── technology/
```

If a new topic category is needed (e.g., `agriculture/`, `health/`), create the subdirectory and update the root `README.md`.

---

## Submitting Your Contribution

1. **Fork** this repository
2. Create a branch: `git checkout -b data/your-dataset-name`
3. Add your CSV file(s) to the appropriate folder
4. Update [DATA_CATALOG.md](DATA_CATALOG.md) with a new row for your dataset
5. Update the folder's `README.md` (or create one if it doesn't exist)
6. Open a **Pull Request** with a description of what the dataset is and where you sourced it

---

## Data Quality Checklist (PR reviewers will check these)

- [ ] File is valid UTF-8 CSV (no encoding errors)
- [ ] Column names are `snake_case`
- [ ] No currency symbols or text mixed into numeric columns
- [ ] Missing values are empty cells, not strings
- [ ] At least one date/year column is present
- [ ] Source is cited in DATA_CATALOG.md
- [ ] Dataset covers at least one African market

---

## Code of Conduct

Be respectful, cite your sources, and prioritize data accuracy. If you are unsure about data quality, open an Issue to discuss before submitting a PR.
