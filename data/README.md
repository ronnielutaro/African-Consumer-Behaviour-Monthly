# Data

All open datasets in this repository are organized here by geographic scope and topic.

## Structure

```
data/
├── uganda/              → Uganda-specific datasets
│   ├── economy/
│   ├── demographics/
│   ├── technology/
│   └── business/
├── east-africa/         → EAC regional datasets
│   ├── economy/
│   ├── demographics/
│   └── technology/
└── africa-wide/         → Pan-African datasets
    ├── economy/
    └── technology/
```

## Browse the Data Catalog

See [DATA_CATALOG.md](../DATA_CATALOG.md) for a full browsable index of all datasets with descriptions, sources, and coverage periods.

## Standards

- File format: **CSV (UTF-8)**
- Date/year: **ISO 8601** (`YYYY`)
- Numeric values: plain numbers, no symbols
- Missing values: **empty cell**
- Country codes: **ISO 3166-1 alpha-3**

See [CONTRIBUTING.md](../CONTRIBUTING.md) for the full standards guide.
