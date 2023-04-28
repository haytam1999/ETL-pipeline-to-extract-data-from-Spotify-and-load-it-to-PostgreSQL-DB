# ETL-pipeline-to-extract-data-from-Spotify-and-load-it-to-PostgreSQL-DB

This project consist of building an ETL pipeline that uses Spotify APIs to move data from the platform to a PostgreSQL Database.

1) Tools used: 

  -Python
  
  -API’s
  
  -Docker
  
  -Airflow
  
  -PostgreSQL
	
2) Data Source:

The data will be extracted from a user account in spotify and loaded to postgreSQL database.

3) Schema:

Here is the schema I followed to build the pipeline:

![alt text](https://github.com/haytam1999/ETL-pipeline-to-extract-data-from-Spotify-and-load-it-to-PostgreSQL-DB/blob/master/Schema.png?raw=true)

4) Scripts:

Extract.py: Extracts the Data from Spotify using a specific Token. 

Transform.py: make transformations on the extracted data.

Load.py: Using sqlalchemy and SQLite to load our data into a database.

Spotify_etl.py: write a logic to extract data from API → Do Quality Checks →Transform Data.
					 
*spotify_final_dag.py: Airflow DAG to orchestrat the process.
