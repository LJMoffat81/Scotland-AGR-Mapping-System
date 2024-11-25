# Scotland AGR Mapping System

The **Scotland AGR Mapping System** is a Python-based tool developed to calculate Annual Ground Rent (AGR) for all land parcels in Scotland. By providing accurate and transparent AGR valuations, this system aims to replace traditional taxes on production and capital, supporting fair land reform and promoting sustainable economic development.

This project is sponsored by the [Scottish Land Revenue Group (SLRG)](https://www.slrg.scot).

## Features
- **Dynamic Grid Management:** Utilises the What3Words API to divide land parcels into easily identifiable units.
- **PostGIS Integration:** Efficiently manages and analyses geospatial data for precise mapping.
- **Custom AGR Algorithm:** Calculates AGR values using weighted factors like land size, location, and usage.
- **Scalable Design:** Built for future expansion and integration with additional datasets.

## About Annual Ground Rent (AGR)

Annual Ground Rent (AGR) is an innovative system of land valuation that replaces traditional taxes. AGR captures the value of land as a shared natural resource, ensuring this wealth is returned to the community while reducing inequality and encouraging sustainable land use.

For more information, visit the [Scottish Land Revenue Group](https://www.slrg.scot).

## Project Structure
```
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

```
## Installation

### Prerequisites
- Python 3.8 or higher - PostgreSQL with PostGIS extension - What3Words API key

### Steps
1. Clone the repository: git clone https://github.com/your-username/AGR-Mapping-System.git cd AGR-Mapping-System 2. Set up a virtual environment and install dependencies: python -m venv venv source venv/bin/activate # On Windows, use `venv\Scripts\activate` pip install -r docs/requirements.txt 3. Configure the database: - Set up PostgreSQL with PostGIS following instructions in docs/database-setup.md. 4. Add your What3Words API key: - Replace your-api-key in src/api/what3words_config.py with your API key.

## Usage
To calculate the AGR for a specific land parcel: python src/main.py --location "three.word.address" Replace three.word.address with a valid What3Words location. For additional options, run: python src/main.py --help

## Contributing
We welcome contributions! Please follow these steps to get involved: 1. Fork the repository. 2. Create a feature branch (git checkout -b feature-name). 3. Commit changes and open a pull request. Before contributing, please review the CONTRIBUTING.md guidelines.

## Roadmap

### Current Goals
- Integrate What3Words API for location handling. - Develop a robust AGR calculation algorithm. - Implement geospatial database integration with PostGIS.
### Future Enhancements
- Add support for additional APIs and datasets. - Develop a web-based UI for user interaction. - Deploy on a cloud platform for wider accessibility.

## Acknowledgements
- [Scottish Land Revenue Group (SLRG)](https://www.slrg.org.uk) for sponsoring this project. - [What3Words](https://what3words.com) for their API integration. - Open source contributors to [PostGIS](https://postgis.net) and Python tools that power this project.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
**Laurie Moffat** For inquiries, please contact [Laurie Moffat](mailto:LJMoffat@protonmail.com).
