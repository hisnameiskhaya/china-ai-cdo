# ChinaAI CDO Data Repository

Repository for managing ChinaAI's tokenized CDO data tracking BRICS exports.

## Structure

```
china-ai-cdo/
├── data/
│   ├── companies/     # Individual company CSVs
│   ├── config/        # Static configurations
│   └── historical/    # Historical data backups
```

## Data Format

### Company Data (CSV)
- `trade_date`: Date of trade (YYYY-MM-DD)
- `receivables_amount`: Amount in base currency
- `due_date`: Payment due date
- `export_growth`: Quarter-on-Quarter growth rate
- `risk_score`: Calculated risk metric

### Configuration (JSON)
Company metadata and risk parameters are stored in `data/config/companies.json`

## Updates
- Data is updated daily at 00:00 UTC
- Historical data is archived monthly
- Export growth rates are calculated quarter-over-quarter

## Usage
This repository serves as the data source for the ChinaAI Webflow site, providing real-time CDO token metrics and export growth tracking.
