# Data Library Analytics pipeline
This is a Python CLI tool to query the [WFP Data Library API](https://datalib.vam.wfp.org/) and export the data into CSV files or an MS SQL database. It performs an ETL (Extract, Transform, Load) process to fetch data from the VAM Data Library, process the data, and load it into a database and/or save it to an Excel file.

This feeds the [Data Library & Data Bridges Analytics Dashboard](https://analytics.wfp.org/#/views/DataLibraryAnalytics/DataBridgesUsage?:iid=1&:redirect=auth)

## Features
- Queries the Data Library API to get information about users, surveys, resources, and container members.
- Exports data to CSV files.
- Uploads data to an MS SQL database.

## Usage
1. Clone this repository
2. Run `uv sync` to install dependencies
3. Get an API key from your Data Library account.
4. Rename the `.env-example` file to `.env`.
5. Add the API key and database credentials to the `.env` file.
6. Run `python main.py` to query the API and export data.
7. Use the `--csv` flag to export data to CSV files (e.g., `python main.py --csv`).
8. Use the `--db` flag to upload data to a database (e.g., `python main.py --db`).
9. The output CSV files will be saved in the `output` folder.

## Requirements
- Python 3.x
- `uv` as package manager

## Documentation
For more details on the Data Library API endpoints, see the [API documentation](http://docs.ckan.org/en/2.11/api/).

## Contributing
Contributions to add more API querying/exporting functionality are welcome!

## License
This project is licensed under the Affero GPL License - see the [LICENSE](LICENSE) file for details.
