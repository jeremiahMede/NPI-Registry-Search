# NPI Registry Search Tool

A Streamlit application for looking up healthcare provider information using the CMS NPPES (National Plan and Provider Enumeration System) API.

## Features

- **Single NPI Lookup** - Get detailed provider information for any NPI number
- **Batch Processing** - Look up multiple NPIs at once via text input or CSV upload
- **Advanced Search** - Search providers by name, organization, location, or specialty
- **Real-Time Data** - Queries the official CMS NPPES API (updated daily)
- **Export Results** - Download results as CSV

## Data Retrieved

For each NPI, the tool retrieves:
- Provider/Organization name
- Entity type (Individual or Organization)
- Practice location and mailing address
- Phone and fax numbers
- Primary taxonomy/specialty
- Authorized official information
- Enumeration date and status
- Doing Business As (DBA) names

## Live Demo

Access the deployed app at: [Streamlit Cloud URL - Add after deployment]

## Run Locally

```bash
# Clone the repository
git clone https://github.com/jeremiahMede/NPI-Registry-Search.git
cd NPI-Registry-Search

# Install dependencies
pip install -r requirements.txt

# Run the app
streamlit run app.py
```

## API Information

This tool uses the [NPPES NPI Registry API v2.1](https://npiregistry.cms.hhs.gov/api-page) operated by the Centers for Medicare & Medicaid Services (CMS).

**Note:** Issuance of an NPI does not ensure or validate that the Health Care Provider is Licensed or Credentialed.

## Requirements

- Python 3.8+
- streamlit
- pandas
- requests

## License

MIT License
