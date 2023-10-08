# execute_all_sql_in_current_folder_to_excel_sheets_using_python

---

# SQL to Excel Data Exporter

## Introduction

The SQL to Excel Data Exporter is a Python script designed to facilitate the export of SQL query results into an Excel file. This tool is especially useful for those who work with Presto Hive databases and need to analyze and visualize the results of multiple SQL queries.

## Features

- **Easy Configuration**: Configure the Presto Hive database connection parameters in the `config.py` file for seamless integration.
  
- **Batch Export**: Export results from multiple SQL files into separate sheets within a single Excel file.
  
- **Versatile Compatibility**: Use this tool with various SQL files containing different queries, making it adaptable to diverse analysis requirements.
  
- **Automated Execution**: Simply run the script, and it will handle the execution, data retrieval, and Excel export processes automatically.
  
## Prerequisites

Before you start using this tool, ensure that you have the following prerequisites installed:

- **Python 3.x**: You can download Python from [python.org](https://www.python.org/downloads/).
  
- **Required Python Libraries**: Install the required libraries using `pip`:

  ```shell
  pip install pyhive pandas openpyxl
  ```

## Configuration

1. **Credentials Configuration**:

   Open the `config.py` file and set the following variables:

   - `presto_host`: Replace with your Presto Hive host IP or hostname.
   - `presto_port`: Replace with the Presto port.
   - `presto_username`: Replace with your Presto username.

2. **SQL Queries**:

   Create one or more `.sql` files in the same directory as the script, each containing an SQL query you want to export to Excel.

## Usage

1. **Running the Script**:

   To execute the script, open a terminal or command prompt and navigate to the directory containing your Python script. Run the following command:

   ```shell
   python your_script_name.py
   ```

   Replace `your_script_name.py` with the name of your Python script.

2. **Exported Excel File**:

   The script will generate an Excel file named `all_sql.xlsx` in the same directory. Each SQL query's result will be stored in a separate sheet within the Excel file.

## Example

Suppose you have multiple SQL queries you want to export and analyze. By following these steps:

1. Configure the `config.py` file with your Presto Hive credentials.

2. Create one or more `.sql` files, each containing a different SQL query.

3. Run the script as mentioned in the "Usage" section.

You can easily export and analyze your SQL query results in a single Excel file.

## Notes

- This tool is primarily intended for educational and analysis purposes. In production environments, consider using more advanced and secure solutions for data management.

- Ensure you have proper access rights and permissions for the Presto Hive database to execute queries successfully.

---

