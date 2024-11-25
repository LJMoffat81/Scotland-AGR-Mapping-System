# Scotland AGR Mapping System

The **Scotland AGR Mapping System** is a Python-based tool designed to calculate Annual Ground Rent (AGR) for all land parcels in Scotland. The system supports land reform by providing fair and transparent AGR valuations, replacing traditional taxes on production and capital.

## Features
- **Dynamic Grid Management:** Utilises the What3Words API to identify and manage land parcels dynamically.
- **PostGIS Integration:** Handles geospatial data efficiently for precise land parcel mapping.
- **Custom AGR Algorithm:** Calculates AGR values based on weighted factors, including land size, location, and use.
- **Scalable Architecture:** Built with scalability in mind for future expansion.

## Project Structure

```bash
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

