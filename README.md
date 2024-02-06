# Mssql-to-Postgres-Full-load

## Overview
This Python project, "Mssql-to-Postgres-Full-load," facilitates the full load of data from Microsoft SQL Server (MSSQL) to PostgreSQL. It is designed to streamline the process of transferring data between these two databases, ensuring a smooth and efficient migration.

## GitHub Repository
The project is hosted on GitHub at the following URL:
[https://github.com/joshua-dada-mayowa/Mssql-to-Postgres-Full-load/](https://github.com/joshua-dada-mayowa/Mssql-to-Postgres-Full-load/)

## Project Files
### 1. `config.ini`
This configuration file plays a crucial role in customizing the migration process. It contains parameters such as database connection details, table mappings, and other settings necessary for the successful execution of the full load.

#### Sample `config.ini`:
```ini
[MSSQL]
server = MSSQL_SERVER_ADDRESS
database = MSSQL_DATABASE_NAME
username = MSSQL_USERNAME
password = MSSQL_PASSWORD

[PostgreSQL]
server = POSTGRES_SERVER_ADDRESS
database = POSTGRES_DATABASE_NAME
username = POSTGRES_USERNAME
password = POSTGRES_PASSWORD

# Add more tables as needed
```

### 2. `full_load.py`
The main Python script responsible for executing the full load process. It utilizes the configuration provided in `config.ini` to establish connections to both MSSQL and PostgreSQL databases, fetch data from MSSQL, and insert it into the corresponding tables in PostgreSQL.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/joshua-dada-mayowa/Mssql-to-Postgres-Full-load.git
   ```

2. Navigate to the project directory:
   ```bash
   cd Mssql-to-Postgres-Full-load
   ```

3. Customize the `config.ini` file with your specific database details and table mappings.

4. Run the `full_load.py` script:
   ```bash
   python full_load.py
   ```

5. Monitor the console for any errors or progress updates during the migration process.

## Contributions
Contributions to enhance the functionality or address issues are welcome. Feel free to fork the repository, make changes, and submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code as needed.

For detailed information on the project and its features, refer to the [GitHub repository](https://github.com/joshua-dada-mayowa/Mssql-to-Postgres-Full-load/).
