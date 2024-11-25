# Scotland AGR Mapping System

The **Scotland AGR Mapping System** is a Python-based tool developed to calculate Annual Ground Rent (AGR) for all land parcels in Scotland. By providing accurate and transparent AGR valuations, this system aims to replace traditional taxes on production and capital, supporting fair land reform and promoting sustainable economic development.

This project is sponsored by the [Scottish Land Revenue Group (SLRG)](https://www.slrg.org.uk).

---

## Features
- **Dynamic Grid Management:** Utilises the What3Words API to divide land parcels into easily identifiable units.
- **PostGIS Integration:** Efficiently manages and analyses geospatial data for precise mapping.
- **Custom AGR Algorithm:** Calculates AGR values using weighted factors like land size, location, and usage.
- **Scalable Design:** Built for future expansion and integration with additional datasets.

---

## About Annual Ground Rent (AGR)

Annual Ground Rent (AGR) is an innovative system of land valuation that replaces traditional taxes. AGR captures the value of land as a shared natural resource, ensuring this wealth is returned to the community while reducing inequality and encouraging sustainable land use.

For more information, visit the [Scottish Land Revenue Group](https://www.slrg.org.uk).

---

## Project Structure

```plaintext
AGR-Mapping-System/
│
├── data/                     # Folder for raw and processed data files
│   ├── raw/                  # Unprocessed data
│   └── processed/            # Cleaned and formatted data
│
├── src/                      # Main source code folder
│   ├── api/                  # API-related scripts (e.g., What3Words integration)
│   ├── database/             # Scripts for managing the PostgreSQL database
│   ├── calculations/         # AGR calculation scripts and algorithms
│   └── utils/                # Helper scripts and utility functions
│
├── tests/                    # Folder for unit and integration tests
│   └── test_calculations.py  # Example test file
│
├── docs/                     # Documentation files
│   └── requirements.txt      # Dependencies file for Python environment
│
├── .gitignore                # Specify files/folders Git should ignore
├── README.md                 # Main project documentation
└── LICENSE                   # License file for your project (optional)
